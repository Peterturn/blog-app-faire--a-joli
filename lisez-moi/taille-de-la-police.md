# Bases de Taille de Texte en CSS

Lors de la conception d'une page web, il est essentiel de comprendre comment dimensionner le texte. Voici quelques éléments de base et les unités de mesure couramment utilisées pour ajuster la taille du texte en CSS.

## Tailles de Texte de Base

### `h1`
Le texte de titre de niveau 1 est généralement utilisé pour les titres principaux de la page. Il est plus grand et plus audacieux que les autres éléments de texte.

### `h2`
Les titres de niveau 2 sont légèrement plus petits que les `h1`, mais restent des titres importants.

### `h3-h6`
Les titres de niveau 2 sont légèrement plus petits que les `h1`, mais restent des titres importants.

### `p`
Les paragraphes sont utilisés pour le contenu principal de la page. Leur taille de texte est généralement plus petite que les titres.

## Unités de Mesure

### `px` (Pixels)
Les pixels sont une unité de mesure absolue. La taille du texte en pixels reste constante, indépendamment des paramètres de l'utilisateur. Cela signifie que le texte en pixels peut sembler petit sur les écrans haute résolution.

### `em`
L'unité `em` est relative à la taille du texte de l'élément parent. Par exemple, si la taille de police de l'élément parent est de 16px, `1em` équivaut à 16px. Si l'élément parent a une taille de police de 20px, `1em` sera de 20px.

### `rem` (Root em)
L'unité `rem` est également relative, mais elle est basée sur la taille de la police de l'élément racine (généralement la balise `<html>`). Cela signifie que la taille du texte en `rem` ne dépend pas de la taille du texte de l'élément parent.

## Exemple d'Utilisation

Pour définir la taille du texte en utilisant `rem`, vous pouvez écrire :

```css
html {
  font-size: 16px; /* Taille de police de base pour 1rem */
}

p {
  font-size: 1.5rem; /* 1.5 fois la taille de police de base */
}

h1 {
  font-size: 2rem; /* 2 fois la taille de police de base */
}

h2 {
  font-size: 1.8rem; /* 1.8 fois la taille de police de base */
}

