---
layout: default
title: Typography
parent: UI Components
nav_order: 1
---

# Typographie
{: .no_toc}

## Table des matières
{: .no_toc .text-delta}

1. COT
{: toc}

---

## Pile de polices

Par défaut, Just the Docs utilise une pile de polices système native pour les polices sans-serif:

```scss
-apple-system, BlinkMacSystemFont, "helvetica neue", helvetica, roboto, noto, "segoe ui", arial, sans serif
```

ABCDEFGHIJKLMNOPQRSTUVWXYZ
abcdefghijklmnopqrstuvwxyz
{: .fs-5 .ls-10 .code-example}

Pour le type monospace, comme les extraits de code ou l'élément `<pre>`, Just the Docs utilise une pile de polices système native pour les polices monospace:

```scss
"SFMono-Regular", Menlo, Consolas, Monospace
```

ABCDEFGHIJKLMNOPQRSTUVWXYZ
abcdefghijklmnopqrstuvwxyz
{: .fs-5 .ls-10 .text-mono .code-example}

---

## échelle de type sensible

Juste la documentation utilise une échelle de type sensible qui change en fonction de la taille de la fenêtre.

| Sélecteur | Petite taille de l'écran `font-size` | Grand écran `font-size` |
|:----------------------|:---------------------------------|:------------------------------|
| `h1`, `.text-alpha`   | 32px                             | 36px                          |
| `h2`, `.text-beta`    | 18px                             | 24px                          |
| `h3`, `.text-gamma`   | 16px                             | 18px                          |
| `h4`, `.text-delta`   | 14px                             | 16px                          |
| `h5`, `.text-epsilon` | 16px                             | 18px                          |
| `h6`, `.text-zeta`    | 18px                             | 24px                          |
| `body`                | 14px                             | 16px                          |

---

## Rubriques

Les titres sont rendus comme ceci:

<div class="code-example">
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>
</div>
```markdown
# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6
```

---

## Body text

Le corps du texte par défaut est rendu comme ceci:

<div class="code-example" markdown="1">
Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
</div>
```markdown
Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
```

---

## Inline elements

<div class="code-example" markdown="1">
Text peut être **bold**, _italic_, or ~~strikethrough~~.

[Link to another page](another-page).
</div>

```markdown
Text peut être **bold**, _italic_, or ~~strikethrough~~.

[Link to another page](another-page).
```

---

## Utilitaires typographiques

Un certain nombre de classes CSS typographiques spécifiques vous permettent de remplacer le style par défaut pour la taille et l'épaisseur de la police, la hauteur de ligne et la capitalisation.

[View typography utilities]({{ site.baseurl }}{% link docs/utilities/utilities.md %}#typography){: .btn .btn-outline }
