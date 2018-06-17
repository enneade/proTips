# Documentation

### HTML5

HTML5 (HyperText Markup Language 5) est la dernière révision majeure du HTML (format de données conçu pour représenter les pages web). Cette version a été finalisée le 28 octobre 2014. HTML5 spécifie deux syntaxes d'un modèle abstrait défini en termes de DOM : **HTML5 et XHTML5**. Le langage comprend également une couche application avec de nombreuses API, ainsi qu'un algorithme afin de pouvoir traiter les documents à la syntaxe non conforme. Le travail a été repris par le W3C en mars 2007 après avoir été lancé par le WHATWG. Les deux organisations travaillent en parallèle sur le même document afin de maintenir une version unique de la technologie. Le W3C clôt les ajouts de fonctionnalités le 22 mai 2011, annonçant une finalisation de la spécification en 20141, et encourage les développeurs Web à utiliser HTML 5 dès ce moment. Fin 2016, la version 5.1 est officiellement publiée et présente plusieurs nouveautés qui doivent faciliter le travail des développeurs d'applications Web2.

* Balises principales
```
<html> // Balise principale
<head> // En-tête de la page
<body> //Corps de la page
<link /> //Liaison avec une feuille de style
<meta /> // Métadonnées de la page web (charset, mots-clés, etc.)
<script> //Code JavaScript
<style> //Code CSS
<title> //Titre de la page
<abbr> // Abréviation
<blockquote> // Citation (longue)
<cite> // Citation du titre d'une œuvre ou d'un évènement
<q> // Citation (courte)
<sup> // Exposant
<sub> // Indice
<strong> // Mise en valeur forte
<em> // Mise en valeur normale
<mark> // Mise en valeur visuelle
<h1> // Titre de niveau 1
<h2> // Titre de niveau 2
<h3> // Titre de niveau 3
<h4> // Titre de niveau 4
<h5> // Titre de niveau 5
<h6> // Titre de niveau 6
<img /> // Image
<figure> // Figure (image, code, etc.)
<figcaption> // Description de la figure
<audio> // Son
<video> // Vidéo
<source> // Format source pour les balises<audio>et<video>
<a> // Lien hypertexte
<br /> // Retour à la ligne
<p> // Paragraphe
<hr /> // Ligne de séparation horizontale
<address> // Adresse de contact
<del> // Texte supprimé
<ins> // Texte inséré
<dfn> // Définition
<kbd> // Saisie clavier
<pre> // Affichage formaté (pour les codes sources)
<progress> // Barre de progression
<time> // Date ou heure
```
### CSS3
Les feuilles de style en cascade, généralement appelées CSS de l'anglais **Cascading Style Sheets**, forment un langage informatique qui décrit la présentation des documents HTML et XML. Les standards définissant CSS sont publiés par le World Wide Web Consortium (W3C). Introduit au milieu des années 1990, CSS devient couramment utilisé dans la conception de sites web et bien pris en charge par les navigateurs web dans les années 2000.
* structure
* Selecteur (div, .nomDiv, .#id)
* Proprieté (ex. color)
* Attribut (ex. red)
```
.nomDiv {
  font-size: 16px;
  }
```

* Exemple HTML et CSS3

<!doctype html>
<html>
    <head>
        <meta charset="utf-8"/>
        <link rel="stylesheet" href="style.css"/>
        <title>Exemple html et css</title>
    </head>
    <body>
        <button class="btn" id="btn1">Premier bouton</button><br/><br/>
        <button class="btn" id="btn2">Deuxième bouton</button><br/><br/>
        <button class="btn" id="btn3">Troisième bouton</button>
    </body>
</html>

.btn{
    height: 50px;
    color: white;
    font-size: 20px;
    cursor: pointer;
    transition: background-color 2s;
    outline: none;
    border: none;
}

.btn:hover{
    transition: background-color 2s;
}
#btn1{
    background-color: lightgreen;
}
#btn1:hover{
    background-color: darkgreen;
}
#btn2{
    background-color: lightblue;
}
#btn2:hover{
    background-color: darkblue;
}
#btn3{
    background-color: red;
}
#btn3:hover{
    background-color: orange;
}
### FONTFACE
La règle @ @font-face permet de définir les polices d'écriture à utiliser pour afficher le texte de pages web. Cette police peut être chargée depuis un serveur distant ou depuis l'ordinateur de l'utilisateur. Si la fonction local() est utilisée, elle indique à l'agent utilisateur de prendre en compte une police présente sur le poste de l'utilisateur.

En permettant aux auteurs de fournir leurs propres polices, il n'est plus nécessaire de dépendre uniquement des polices qui sont installées sur les postes des utilisateurs.

Il est courant d'utiliser les deux formes url() et local() afin de pouvoir utiliser une police locale si elle est disponible ou d'en télécharger une autre au cas où.

La règle @font-face peut être utilisée au niveau global d'une feuille de style et également au sein d'un groupe lié à une règle @ conditionnelle.

* Préséparation
Dans un premier temps, il faut préparer notre font, dans tous les formats nécessaires.
Les trois formats principaux (les plus couramment utilisés sur le web) sont les suivants : **SVG** (Scalable Vector Graphics), **TTF** (True Type Font) et **EOT** (Embedded Open Type).
Pour une police, il peut y avoir plusieurs variations : Gras, Italique, light, etc.
Il faudra donc préparer nos fichiers, avec les bonnes variations et les bonnes extensions.
Pour notre exemple, nous allons prendre une police “fictive” appelée LOVEP.
Nous allons donc préparer les fichiers de cette Font LOVEP en gras et en normal, dans les formats TTF et EOT (pour IE9), et nous aurons donc les fichiers suivants :

LOVEP.ttf
LOVEP.eot
LOVEPbold.ttf
LOVEPbold.eot

Si la font téléchargée n’a pas tous ces formats, il existe des convertisseurs de format de police, comme Free Font Converter ou encore Online Font Converter.
Une fois ces fichiers préparés, il faut les uploader (par FTP) dans le dossier de notre thème, à la racine ou dans un sous dossier selon notre choix. Dans cet exemple, nous allons les placer à la racine du thème.


### FLEXBOXGRID
FlexBox (pourFlexible Box) est un mode de mise en page prévoyant une disposition des éléments d’une page de telle sorte que ces éléments possèdent un comportement prévisible lorsqu’ils doivent s’accommoder de différentes tailles d’écrans/appareils. Dans de nombreux cas, le modèle de boîte Flexbox offre une amélioration du modèle block dans lequel les flottements (float) ne sont pas utilisés, pas plus que la fusion des marges du conteneur flexible avec ses éléments.

Les éléments enfants d’une flexbox peuvent être placés dans n’importe quelle direction et peuvent avoir des dimensions pour s'adapter à la place disponible. Positionner les éléments enfants est ainsi plus simple et les agencements complexes peuvent être mis en place plus simplement et avec un code plus propre, étant donné que l'ordre d'affichage des éléments est indépendant de leur ordre dans le code source.

* Grid
Une grille est un ensemble de lignes horizontales et verticales qui se croisent – les premières définissant les rangées, et les secondes les colonnes. Les éléments sont placés sur la grille en fonction de ces rangées et colonnes. Les fonctionnalités sont les suivantes :

**Pistes à taille fixe ou variable**
On peut créer une grille avec des pistes à taille fixes en utilisant une unité comme le pixel. Pour les pistes à taille variable on peut utiliser le pourcentage ou la nouvelle unité fr créée à cet effet.

**Placement des éléments**
Pour placer les éléments sur la grille, on peut utiliser le numéro ou le nom d'une ligne, ou cibler une zone particulière. La grille contient aussi un algorithme pour placer les éléments qui n'ont pas été placés explicitement.

**Création de pistes supplémentaires pour du contenu**
Lorsqu'une grille explicite n'est pas définie, la spécification prend en charge le contenu défini en dehors d'une grille en ajoutant des colonnes et des rangées. Cela comprend des fonctionnalités telles qu'« ajouter autant de colonnes que possible dans le conteneur ».

**Contrôle de l'alignement**
On peut contrôler l'alignement des éléments dans une zone de la grille, ainsi que celui de l'ensemble de la grille.

**Contrôle des contenus qui se chevauchent**
Il peut arriver que l'on place plusieurs éléments dans une même cellule, ou que des zones se chevauchent. La superposition peut être contrôlée à l'aide de la propriété z-index.

La grille est une spécification puissante qui peut être combinée avec d'autres modules CSS tels que flexbox. Le point de départ est le conteneur.

### SCSS/SASS

* SCSS

  * Possibilité d'embriquer les selecteurs pour respecter le niveau de hiérarchie
  * Création de conditions, boucles et mixins (responsive)
  * Possibilité d'utiliser des variables

```
.jeSuisParent{
  color: $someColor; // VARIABLE

.jeSuisEnfant {
  color: yellow;
  }
}
```

* SASS :
Sass (Syntactically Awesome Stylesheets) est un langage de génération de feuilles de style initialement développé par Hampton Catlin et Nathalie Weizenbaum.
Sass est un langage de feuilles de style en cascade (CSS). C'est un langage de description qui est compilé en CSS. SassScript est un langage de script pouvant être utilisé à l’intérieur du code Sass. Deux syntaxes existent. La syntaxe originale, nommée « syntaxe indentée », est proche de Haml. La nouvelle syntaxe se nomme SCSS. Elle a un formalisme proche de CSS.

Mêmes carcatéristiques que le SCSS, mais différences à niveau syntaxique: alors que le SCSS respecte l'utilisation des accolades et des points virgules comme en CSS classique, en SASS il n'y a ni d'accolades ni de points virgules, ainsi la hiérarchie est gerée par l'indentation (comme en PUG, voir ci-dessus).

Exemple

```
.jeSuisParent
  color: $someColor

  .jeSuisEnfant
    color: yellow
```
### Sites de veilles

* [Medium](https://medium.com)
* [Awwwards](https://www.awwwards.com)
* [Codepen](https://codepen.io)
* [JDN](https://www.journaldunet.com/)
* [UX Planet](https://uxplanet.org/)

### Sites indispensables
* [W3C](https://www.w3.org/)
* [MDN](https://developer.mozilla.org/fr/)
