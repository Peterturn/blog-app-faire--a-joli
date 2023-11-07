# Sélecteurs CSS

1. **Sélecteur Universel :**
   - `*` - Sélectionne tous les éléments de la page.

2. **Sélecteur de Type :**
   - `élément` - Sélectionne tous les éléments d'un type spécifique, par exemple, `p` sélectionne tous les éléments `<p>, <h1>, <h2>, <p>, <div>, <main>, <header> ...`.

3. **Sélecteur de Classe :**
   - `.classe` - Sélectionne tous les éléments avec une classe spécifique, par exemple, `.btn` sélectionne tous les éléments avec `class="btn"`.

4. **Sélecteur d'ID :**
   - `#id` - Sélectionne un élément unique avec un attribut `id` spécifique, par exemple, `#header` sélectionne l'élément avec `id="header"`.

5. **Sélecteur Descendant :**
   - `élément élément` - Sélectionne un élément qui est un descendant d'un autre élément, par exemple, `ul li` sélectionne tous les éléments `<li>` à l'intérieur d'un `<ul>`.

6. **Sélecteur Enfant :**
   - `parent > enfant` - Sélectionne un élément enfant qui est un enfant direct d'un élément parent, par exemple, `nav > ul` sélectionne tous les éléments `<ul>` qui sont des enfants directs de `<nav>`.

7. **Sélecteur Frère Adjacent :**
   - `élément + élément` - Sélectionne un élément qui est immédiatement précédé d'un autre élément, par exemple, `h2 + p` sélectionne un `<p>` immédiatement après un `<h2>`.

8. **Sélecteur Frère Général :**
   - `élément ~ élément` - Sélectionne les éléments frères d'un autre élément partageant le même parent, par exemple, `h2 ~ p` sélectionne tous les `<p>` qui sont des frères d'un `<h2>`.

9. **Sélecteur d'Attribut :**
   - `[attribut]` - Sélectionne les éléments avec un attribut spécifique, par exemple, `[data-toggle]` sélectionne tous les éléments avec l'attribut `data-toggle`.

10. **Sélecteur d'Attribut avec Valeur :**
    - `[attribut="valeur"]` - Sélectionne les éléments avec un attribut et une valeur spécifiques, par exemple, `[type="text"]` sélectionne tous les éléments avec `type="text"`.

11. **Sélecteur d'Attribut qui Commence par :**
    - `[attribut^="valeur"]` - Sélectionne les éléments avec un attribut qui commence par une valeur spécifique, par exemple, `[href^="https"]` sélectionne tous les éléments avec `href` commençant par "https".

12. **Sélecteur d'Attribut qui se Termine par :**
    - `[attribut$="valeur"]` - Sélectionne les éléments avec un attribut qui se termine par une valeur spécifique, par exemple, `[src$=".jpg"]` sélectionne tous les éléments avec `src` se terminant par ".jpg".

13. **Sélecteur d'Attribut qui Contient :**
    - `[attribut*="valeur"]` - Sélectionne les éléments avec un attribut contenant une valeur spécifique, par exemple, `[class*="btn"]` sélectionne tous les éléments avec `class` contenant "btn".

14. **Sélecteurs Pseudo-Classes :**
    - `:pseudo-classe` - Sélectionne les éléments en fonction de leur état ou condition, par exemple, `:hover` sélectionne les éléments lorsqu'ils sont survolés.

15. **Sélecteurs Pseudo-Éléments :**
    - `::pseudo-élément` - Sélectionne une partie d'un élément, par exemple, `::before` crée un pseudo-élément pour le contenu d'un élément avant lui.

16. **Sélecteur de Groupe :**
    - `sélecteur1, sélecteur2` - Sélectionne plusieurs éléments en utilisant une liste séparée par des virgules, par exemple, `h1, h2, h3` sélectionne tous les éléments `<h1>`, `<h2>`, et `<h3>`.

Ce sont quelques-uns des sélecteurs CSS couramment



## la "cascade" de Sélecteurs CSS

En CSS, lorsque plusieurs sélecteurs ciblent le même élément ou la même propriété, la spécificité et l'ordre de la source déterminent la règle qui a la priorité, ce qui est souvent appelé "spécificité" et "cascade".

Spécificité : La spécificité est une mesure du degré de spécificité d'un sélecteur. Elle est généralement représentée par une valeur en quatre parties (a, b, c, d), où chaque partie correspond à différents composants du sélecteur. Le sélecteur ayant la valeur de spécificité la plus élevée est prioritaire. Par exemple, un style en ligne (spécificité la plus élevée) l'emporte sur un sélecteur de classe.

Ordre des sources : Si deux sélecteurs ont la même spécificité, celui qui apparaît le plus tard dans le document CSS est prioritaire. C'est ce que l'on appelle la "cascade" de CSS.

Voici l'ordre d'importance, du plus élevé au plus bas :

Les styles en ligne : Ils ont la spécificité la plus élevée et ont donc la priorité sur tous les autres styles.
ID : Les sélecteurs d'ID sont très spécifiques et ont la priorité sur les sélecteurs de classes ou d'éléments.
Classes, attributs et pseudo-classes : Ces sélecteurs sont considérés comme les suivants en termes de spécificité.
Éléments et pseudo-éléments : Ces sélecteurs ont la spécificité la plus faible.
Par exemple, considérons le CSS suivant :