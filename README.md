## Résumé Complet de HTML

### 1. Structure de Document HTML5

Chaque document HTML commence par la déclaration de type `<!DOCTYPE html>`, indiquant au navigateur qu'il s'agit d'un document HTML5. Voici la structure de base :

```html
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Titre de la Page</title>
</head>
<body>
    <!-- Contenu de la page -->
</body>
</html>
```

### 2. Balises Essentielles HTML

#### 2.1 Structure et Texte
- **`<h1> - <h6>`** : Titres (de `<h1>` le plus important à `<h6>` le moins important).
- **`<p>`** : Paragraphe de texte.
- **`<br>`** : Saut de ligne (autonome).
- **`<hr>`** : Ligne horizontale pour séparer les sections.

#### 2.2 Conteneurs et Organisation
- **`<div>`** : Conteneur de bloc polyvalent.
- **`<span>`** : Conteneur en ligne pour styliser une partie de texte.

#### 2.3 Médias et Liens
- **`<a href="URL">...</a>`** : Hyperlien, avec `target="_blank"` pour ouvrir dans un nouvel onglet.
- **`<img src="image.jpg" alt="Description de l'image">`** : Image, avec `alt` pour l'accessibilité.
- **`<audio>` et `<video>`** : Éléments multimédias, avec attributs comme `controls`, `autoplay`, `loop`.

#### 2.4 Listes
- **`<ul>`** : Liste non ordonnée (à puces) contenant des `<li>`.
- **`<ol>`** : Liste ordonnée (numérotée) contenant des `<li>`.
- **`<li>`** : Élément de liste.

#### 2.5 Tableaux
- **`<table>`** : Conteneur principal pour un tableau.
- **`<tr>`** : Ligne du tableau.
- **`<td>`** : Cellule de données.
- **`<th>`** : En-tête de tableau.

#### 2.6 Formulaires et Interactions Utilisateur
- **`<form action="URL" method="POST/GET">...</form>`** : Formulaire HTML.
- **`<input type="text">`** : Champs de texte.
- **`<button>`** : Bouton de soumission.
- **`<select>`** : Liste déroulante avec des `<option>`.
- **`<label for="id">`** : Étiquette pour associer le texte à un élément de formulaire, améliorant l'accessibilité.

### 3. Attributs HTML

Les attributs ajoutent des informations supplémentaires à une balise :

- **`id`** : Identifiant unique pour l’élément.
- **`class`** : Classe pour appliquer des styles à plusieurs éléments.
- **`src`** : Spécifie la source d’un fichier (images, scripts).
- **`href`** : URL cible d’un lien `<a>`.
- **`alt`** : Texte alternatif pour les images.

### 4. Balises Sémantiques HTML5

HTML5 a introduit des balises sémantiques pour améliorer l'organisation et l'accessibilité des pages :

- **`<header>`** : Section d'en-tête pour titres et navigation.
- **`<footer>`** : Section de pied de page pour informations de contact.
- **`<nav>`** : Contient des liens de navigation.
- **`<article>`** : Contenu indépendant, comme un article de blog.
- **`<section>`** : Section thématique.
- **`<aside>`** : Informations complémentaires ou barre latérale.
- **`<main>`** : Contenu principal de la page.

<hr>

## Résumé Complet de CSS

### 1. Inclusion de CSS
- **En ligne** : 
  - Utilise l'attribut `style` dans les balises HTML pour des styles spécifiques à un élément.
  
- **Interne** : 
  - Utilise la balise `<style>` dans la section `<head>` du document HTML pour des styles applicables uniquement à cette page.
  
- **Externe** : 
  - Crée un fichier CSS séparé et l'inclut avec `<link rel="stylesheet" href="style.css">`. Cette méthode est la plus efficace pour le réemploi des styles sur plusieurs pages.

### 2. Sélecteurs CSS
- **Type** : Cible tous les éléments d'un type (ex. : `div`, `p`).
- **Classe** : Cible les éléments ayant une classe spécifique (ex. : `.ma-classe`).
- **Identifiant** : Cible un élément avec un identifiant unique (ex. : `#mon-id`).
- **Combinés** : Cible des éléments selon leur relation (ex. : `div p` cible tous les `<p>` dans des `<div>`).
- **Attribut** : Cible les éléments selon la présence ou la valeur d'un attribut (ex. : `input[type="text"]`).
- **Pseudo-classes** : Cible les éléments dans des états spécifiques (ex. : `:hover`, `:first-child`).
- **Pseudo-éléments** : Cible des parties spécifiques d'un élément (ex. : `::before`, `::after`).

### 3. Propriétés CSS
- **Couleur et Fond** :
  - `color` : Définit la couleur du texte.
  - `background-color` : Définit la couleur d'arrière-plan.
  - `background-image` : Définit une image d'arrière-plan.

- **Typographie** :
  - `font-size` : Taille de la police.
  - `font-family` : Type de police à utiliser.
  - `font-weight` : Épaisseur de la police (normal, bold).
  - `line-height` : Hauteur de ligne pour l'espacement vertical.

- **Marge et Remplissage** :
  - `margin` : Espace extérieur autour d'un élément.
  - `padding` : Espace intérieur entre le contenu et la bordure.
  - `margin-top`, `margin-right`, `margin-bottom`, `margin-left` : Contrôle des marges individuelles.

- **Dimension** :
  - `width` : Largeur de l’élément.
  - `height` : Hauteur de l’élément.
  - `max-width` / `max-height` : Dimensions maximales.
  - `min-width` / `min-height` : Dimensions minimales.

- **Bordure** :
  - `border` : Définit le style, la largeur et la couleur de la bordure.
  - `border-radius` : Arrondit les coins d'un élément.
  - `border-style`, `border-width`, `border-color` : Propriétés individuelles pour la bordure.

- **Affichage** :
  - `display` : Définit comment un élément est affiché (block, inline, flex, grid, none).
  - `position` : Définit la méthode de positionnement (static, relative, absolute, fixed, sticky).
  - `z-index` : Définit l'ordre d'empilement des éléments.

- **Autres propriétés** :
  - `opacity` : Définit la transparence d'un élément.
  - `overflow` : Contrôle le comportement lorsque le contenu déborde (visible, hidden, scroll, auto).
  - `box-shadow` : Ajoute une ombre à un élément.
  - `transition` : Gère les transitions de propriété CSS.

### 4. Modèle de Boîte
- **Structure** :
  - **Contenu** : Le contenu réel de l'élément.
  - **Padding** : Espace entre le contenu et la bordure.
  - **Bordure** : La ligne qui entoure l'élément.
  - **Margin** : Espace extérieur autour de l'élément.

### 5. Responsive Design
- **Unités relatives** : Utilisation de `em`, `rem`, `vw`, `vh`, et `%` pour une mise en page adaptable.
- **Media Queries** : Permet d'appliquer des styles conditionnels en fonction de la taille de l'écran.


<hr>
<h3 align="center"> 🧑🏻‍💻 | Made By : <a href="https://github.com/mohamedtalhaouii" target="_blank">Mohamed Talhaoui</a></h3>
