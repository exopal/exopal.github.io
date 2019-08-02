---
layout: default
title: Acceuil
nav_order: 1
description: "Documentation pour site exopack."
permalink: /
---

# C'est quoi
{: .fs-9 }


 Générateur de site static pour la documentatoin du projet Exopal avec Jekyll, Jekyll est un générateur de site statique simple, compatible avec les blogs. Il prend un répertoire de modèles contenant des fichiers de texte brut dans divers formats, l'exécute via un convertisseur (comme Markdown) et son moteur de rendu Liquid, et crée un site Web statique complet et prêt à être publié pour servir avec votre serveur Web préféré.
 {: .fw-400 .fs-5 }


Le site Web de Jekyll se trouve à l'adresse http://jekyllrb.com/ , et la documentation peut être consultée à l' adresse http://jekyllrb.com/docs/home/ . 



# Table des matières
{: .no_toc .text-delta}

1. COT
{: toc}


---

# Typographie (composant UI)
{: .fs-9 }

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


# Étiquettes (composant UI)
{: .fs-9 }

Utilisez des étiquettes pour ajouter une marque supplémentaire à une section de vos documents. Les étiquettes sont disponibles en quelques couleurs. Par défaut, les étiquettes seront bleues.

<div class="code-example" markdown = "1">
Étiquette par défaut
{: .label}

Étiquette bleu
{: .label .label-blue}

Stable
{: .label .label-green}

Nouvelle version
{: .label .label-purple}

Arrive bientôt
{: .label .label-yellow}

Obsolète
{: .label .label-red}
</div>

```markdown
Étiquette par défaut
{: .label}

Étiquette bleu
{: .label .label-blue}

Stable
{: .label .label-green}

Nouvelle version
{: .label .label-purple}

Arrive bientôt
{: .label .label-yellow}

Obsolète
{: .label .label-red}

```

# Les tables (composant UI)
{: .fs-9 }

Les tables sont réactives par défaut, ce qui permet aux tables larges d'avoir un défilement horizontal pour accéder aux colonnes en dehors de la fenêtre d'affichage normale.

<div class="code-example" markdown="1">

| entete       | entete 2          | 3     |
|:-------------|:------------------|:------|
| ok           | good swedish fish | nice  |
| out of stock | good and plenty   | nice  |
| ok           | good `oreos`      | hmm   |
| ok           | good `zoute` drop | yumm  |

</div>

```markdown
| entete       | entete 2          | 3     |
|:-------------|:------------------|:------|
| ok           | good swedish fish | nice  |
| out of stock | good and plenty   | nice  |
| ok           | good `oreos`      | hmm   |
| ok           | good `zoute` drop | yumm  |
```

# Lists (composant UI)
{: .fs-9 }



La plupart des listes peuvent être rendues avec Markdown pur.

## Liste non ordonnée

<div class="code-example" markdown="1">
- Item 1
- Item 2
- Item 3

_or_

* Item 1
* Item 2
* Item 3
</div>
```markdown
- Item 1
- Item 2
- Item 3

_or_

* Item 1
* Item 2
* Item 3
```

## Liste ordonnée

<div class="code-example" markdown="1">
1. Item 1
1. Item 2
1. Item 3
</div>
```markdown
1. Item 1
1. Item 2
1. Item 3
```

## Task list
{: .fs-9 }

<div class="code-example" markdown="1">
- [ ] bonjour, ceci est une tâche
- [ ] bonjour, ceci est un autre article à faire
- [x] au revoir, cet objet est terminé
</div>

```markdown
- [ ] bonjour, ceci est une tâche
- [ ] bonjour, ceci est un autre article à faire
- [x] au revoir, cet objet est terminé
```

## Liste de définition

Les listes de définitions nécessitent la syntaxe HTML et ne sont pas prises en charge par le compilateur GitHub Flavored Markdown.

<div class="code-example" markdown="1">
<dl>
<dt>Name</dt>
<dd>Godzilla</dd>
<dt>Born</dt>
<dd>1952</dd>
<dt>Birthplace</dt>
<dd>Japan</dd>
<dt>Color</dt>
<dd>Green</dd>
</dl>
</div>

```html

<dl>
  <dt>Name</dt>
  <dd>Godzilla</dd>
  <dt>Born</dt>
  <dd>1952</dd>
  <dt>Birthplace</dt>
  <dd>Japan</dd>
  <dt>Color</dt>
  <dd>Green</dd>
</dl>

```

# Code (composant UI)
{: .no_toc}



## code en ligne

Le code peut être rendu en ligne en l’enveloppant dans des ticks simples.

<div class="code-example" markdown = "1">
Lorem ipsum dolor sit amet, `<extrait de code en ligne>` élit adipisicing, fait une incursion temporelle dans le travail et dolore magna aliqua.
</div>
```markdown
Lorem ipsum dolor sit amet, `<extrait de code en ligne>` élit adipisicing, fait une incursion temporelle dans le travail et dolore magna aliqua.
```

---

## Syntax en surbrillance des blocs de code

Utilisez la syntaxe intégrée de Jekyll en mettant en surbrillance Rouge pour les blocs de code en utilisant trois backticks, suivis du nom de la langue:

<div class="code-example" markdown = "1">
```js
// code Javascript avec coloration syntaxique.
var fun = fonction lang (l) {
  dateformat.i18n = require ('./lang/' + l)
  retourne vrai;
}

```
</div>
{% highlight markdown %}
```js
// code Javascript avec coloration syntaxique.
var fun = fonction lang (l) {
  dateformat.i18n = require ('./lang/' + l)
  retourne vrai;
}
```
{% endhighlight %}

---

## Blocs de code avec des exemples rendus

Pour illustrer le code frontal, il est parfois utile d’afficher un exemple de rendu de ce code. Après avoir inclus les styles de votre projet dont vous aurez besoin pour afficher le rendu, vous pouvez utiliser un `<div>` avec la classe `code-example`, suivi de la syntaxe du bloc de code. Si vous voulez rendre votre sortie avec Markdown au lieu de HTML, utilisez l'attribut `markdown =" 1 "` pour indiquer à Jekyll que le code que vous restiturez sera au format Markdown ... Ceci est sur le point d'être méta ...

<div class="code-example" markdown = "1">

<div class="code-example" markdown = "1">

[button de lien](http://example.com/){: .btn}

</div>

```markdown
[button de lien](http://example.com/){: .btn}
```

</div>
{% highlight markdown %}
<div class="code-example" markdown = "1">

[button de lien](http://example.com/){: .btn}

</div>

```markdown
[button de lien](http://example.com/){: .btn}
```

{% endhighlight %}

# buttons  (composant UI)
{: .fs-9 }


## Styles de buttons de base

### Des liens qui ressemblent à des buttons

<div class="code-example" markdown="1"> 

[Link button](http://example.com/){: .btn}

[button de lien](http://example.com/){: .btn .btn-purple}

[button de lien](http://example.com/){: .btn .btn-blue}

[button de lien](http://example.com/){: .btn .btn-green}

[button de lien](http://example.com/){: .btn .btn-outline}

</div>

```markdown
[button de lien](http://example.com/){: .btn}

[button de lien](http://example.com/){: .btn .btn-purple}

[button de lien](http://example.com/){: .btn .btn-blue}

[button de lien](http://example.com/){: .btn .btn-green}

[button de lien](http://example.com/){: .btn .btn-outline}
```

### Elément Button

GitHub Flavored Markdown ne supporte pas l'élément `button`, vous devrez donc utiliser du HTML intégré pour cela:

<div class="code-example">
<button type="button" name="button" class="btn"> Elément de button </button>
</div>

```html
<button type="button" nom = "button" class="btn"> Elément de button </button>
```


## Utiliser des utilitaires avec des buttons

### Taille du button

Enveloppez le button dans un conteneur qui utilise les [classes d’utilitaires de taille de police]({{site.baseurl}} {% link docs/utilities/typography.md%}) pour redimensionner les buttons:

<div class="code-example" markdown = "1">
<span class="fs-6">
[button gros cul](http://example.com/){: .btn}
</span>

<span class="fs-3">
[Petit button de cul](http://example.com/){: .btn}
</span>
</div>

```markdown
<span class="fs-8">
[button de lien](http://example.com/){: .btn}
</span>

<span class="fs-3">
[Petit button de cul](http://example.com/){: .btn}
</span>

```

### Espacement entre les buttons

Utilisez les [classes d’utilitaires de marge]({{site.baseurl}} {% link docs/utilities/layout.md%} # spacing) pour ajouter un espacement entre deux buttons du même bloc.

<div class="code-example" markdown = "1">
[button avec espace](http://example.com/){: .btn .btn-purple .mr-2}
[Button](http://example.com/){: .btn .btn-blue .mr-2}

[button avec plus d'espace](http://example.com/){: .btn .btn-green .mr-4}
[Button](http://example.com/){: .btn .btn-blue}
</div>

```markdown
[button avec espace](http://example.com/){: .btn .btn-purple .mr-2}
[Button](http://example.com/){: .btn .btn-blue}

[button avec plus d'espace](http://example.com/){: .btn .btn-green .mr-4}
[Button](http://example.com/){: .btn .btn-blue}
```

# buttons
{: .fs-9 }


## Styles de buttons de base

### Des liens qui ressemblent à des buttons

<div class="code-example" markdown = "1">
[button de lien](http://example.com/){: .btn}

[button de lien](http://example.com/){: .btn .btn-purple}
[button de lien](http://example.com/){: .btn .btn-blue}
[button de lien](http://example.com/){: .btn .btn-green}

[button de lien](http://example.com/){: .btn .btn-outline}
</div>

```markdown
[button de lien](http://example.com/){: .btn}

[button de lien](http://example.com/){: .btn .btn-purple}
[button de lien](http://example.com/){: .btn .btn-blue}
[button de lien](http://example.com/){: .btn .btn-green}

[button de lien](http://example.com/){: .btn .btn-outline}
```

### Elément Button

GitHub Flavored Markdown ne supporte pas l'élément `button`, vous devrez donc utiliser du HTML intégré pour cela:

<div class="code-example">
    <button type="button" name="button" class="btn">Elément de button</button>
</div>

```html
<button type="button" name="button" class="btn"> Elément de button </button>

```

## Utiliser des utilitaires avec des buttons

### Taille du button

Enveloppez le button dans un conteneur qui utilise les [classes d’utilitaires de taille de police]({{site.baseurl}} {% link docs/utilities/typography.md %}) pour redimensionner les buttons:

<div class="code-example" markdown = "1">
<span class="fs-6">
[button gros cul](http://example.com/){: .btn}
</span>

<span class="fs-3">
[Petit button de cul](http://example.com/){: .btn}
</span>
</div>

```markdown

<span class="fs-8">
[button de lien](http://example.com/){: .btn}
</span>

<span class="fs-3">
[Petit button de cul](http://example.com/){: .btn}
</span>

```

### Espacement entre les buttons

Utilisez les [classes d’utilitaires de marge]({{ site.baseurl }}{% link docs/utilities/layout.md %}#spacing)  pour ajouter un espacement entre deux buttons du même bloc.

<div class="code-example" markdown="1">

[Button avec espace](http://example.com/){: .btn .btn-purple .mr-2}
[Button](http://example.com/){: .btn .btn-blue .mr-2}

[Button avec plus d'espace](http://example.com/){: .btn .btn-green .mr-4}
[Button](http://example.com/){: .btn .btn-blue}
</div>

```markdown
[Button avec espace](http://example.com/){: .btn .btn-purple .mr-2}
[Button](http://example.com/){: .btn .btn-blue}

[button avec plus d'espace](http://example.com/){: .btn .btn-green .mr-4}
[Button](http://example.com/){: .btn .btn-blue}
```

# Utilities
{: .fs-9 }

Les classes d'utilitaires CSS sont pratiques lorsque vous souhaitez remplacer les styles par défaut pour créer des espaces supplémentaires (marges / marges), corriger les modifications inattendues de la taille ou de l'épaisseur de la police, ajouter de la couleur ou masquer (ou afficher) des éléments d'une taille d'écran spécifique.
{: .fs-6 .fw-300}

# Responsive modifiers
{: .fs-9 }

Seul l'espacement de la documentation fonctionne avec une variété de modificateurs qui vous permettent de cibler en réponse des tailles d'écran spécifiques. Utilisez-les conjointement avec les classes d'espacement et d'affichage de préfixes et suffixes.

| Modifier  | Taille écran                         |
|:----------|:-------------------------------------|
| (none)    | All screens until the next modifier  |
| `xs`      | 320px (20rem) and up                 |
| `sm`      | 500px (31.25rem) and up              |
| `md`      | 740px (46.25rem) and up              |
| `lg`      | 1120px (70rem) and up                |
| `xl`      | 1400px (87.5rem) and up              |


# Layout Utilities
{: .fs-9 }


## Espacement

Ces entretoises peuvent être utilisées pour les marges et le remplissage avec des classes utilitaires réactives. Combinez ces préfixes avec une taille d'écran et une échelle d'espacement pour les utiliser de manière réactive.

| Classname prefix | Ce qu'il fait                 |
|:-----------------|:------------------------------|
| `.m-`            | `margin`                      |
| `.mx-`           | `margin-left`, `margin-right` |
| `.my-`           | `margin top`, `margin bottom` |
| `.mt-`           | `margin-top`                  |
| `.mr-`           | `margin-right`                |
| `.mb-`           | `margin-bottom`               |
| `.ml-`           | `margin-left`                 |

| Classname prefix | Ce qu'il fait                   |
|:-----------------|:--------------------------------|
| `.p-`            | `padding`                       |
| `.px-`           | `padding-left`, `padding-right` |
| `.py-`           | `padding top`, `padding bottom` |
| `.pt-`           | `padding-top`                   |
| `.pr-`           | `padding-right`                 |
| `.pb-`           | `padding-bottom`                |
| `.pl-`           | `padding-left`                  |

Spacing values are based on a `1rem = 16px` spacing scale, broken down into these units:

| Spacer/suffix  | Size in rems  | Rem converted to px |
|:---------------|:--------------|:--------------------|
| `1`            | 0.25rem       | 4px                 |
| `2`            | 0.5rem        | 8px                 |
| `3`            | 0.75rem       | 12px                |
| `4`            | 1rem          | 16px                |
| `5`            | 1.5rem        | 24px                |
| `6`            | 2rem          | 32px                |
| `7`            | 2.5rem        | 40px                |
| `8`            | 3rem          | 48px                |

#### Examples
{: .no_toc }

Le Markdown, utilise le `{: }` wrapper pour appliquer des classes personnalisées:

```markdown
Ce paragraphe aura une marge inférieure de 1rem / 16px sur les grands écrans.
{: .mb-lg-4 }

Ce paragraphe aura un remplissage de 2rem / 32px à droite et à gauche pour toutes les tailles d’écran.
{: .px-6 }
```

## Alignment Vertical

| Class nom              | Ce qu'il fait                   |
|:-----------------------|:--------------------------------|
| `.v-align-baseline`    | `vertical-align: baseline`      |
| `.v-align-bottom`      | `vertical-align: bottom`        |
| `.v-align-middle`      | `vertical-align: middle`        |
| `.v-align-text-bottom` | `vertical-align: text-bottom`   |
| `.v-align-text-top`    | `vertical-align: text-top`      |
| `.v-align-top`         | `vertical-align: top`           |

## Affichage

Les classes d’affichage aident à adapter la disposition des éléments sur une page:

| Class             |                         |
|:------------------|:------------------------|
| `.d-block`        | `display: block`        |
| `.d-flex`         | `display: flex`         |
| `.d-inline`       | `display: inline`       |
| `.d-inline-block` | `display: inline-block` |
| `.d-none`         | `display: none`         |

Utilisez ces classes conjointement avec les modificateurs responsive.

#### Examples
{: .no_toc }

In Markdown, use the `{: }` wrapper to apply custom classes:

```markdown
This button will be hidden until medium screen sizes:

[ A button ](#url)
{: .d-none .d-md-inline-block }

These headings will be `inline-block`:

### heading 3
{: .d-inline-block }

### heading 3
{: .d-inline-block }
```


# Color Utilities
{: .fs-9 }


All the colors used in Just the Docs have been systematized into a series of variables that have been extended to both font color and background color utility classes.

## Light Greys

| Color value    | Font color utility   | Background color utility |
|:---------------|:---------------------|:-------------------------|
| <span class="d-inline-block p-2 mr-1 v-align-middle bg-grey-lt-000"></span> `grey-lt-000` | `.text-grey-lt-000` | `.bg-grey-lt-000` |
| <span class="d-inline-block p-2 mr-1 v-align-middle bg-grey-lt-100"></span> `grey-lt-100` | `.text-grey-lt-100` | `.bg-grey-lt-100` |
| <span class="d-inline-block p-2 mr-1 v-align-middle bg-grey-lt-200"></span> `grey-lt-200` | `.text-grey-lt-200` | `.bg-grey-lt-200` |
| <span class="d-inline-block p-2 mr-1 v-align-middle bg-grey-lt-300"></span> `grey-lt-300` | `.text-grey-lt-300` | `.bg-grey-lt-300` |

## exopal Greys

| Color value    | Font color utility   | Background color utility |
|:---------------|:---------------------|:-------------------------|
| <span class="d-inline-block p-2 mr-1 v-align-middle bg-grey-dk-000"></span> `grey-dk-000` | `.text-grey-dk-000` | `.bg-grey-dk-000` |
| <span class="d-inline-block p-2 mr-1 v-align-middle bg-grey-dk-100"></span> `grey-dk-100` | `.text-grey-dk-100` | `.bg-grey-dk-100` |
| <span class="d-inline-block p-2 mr-1 v-align-middle bg-grey-dk-200"></span> `grey-dk-200` | `.text-grey-dk-200` | `.bg-grey-dk-200` |
| <span class="d-inline-block p-2 mr-1 v-align-middle bg-grey-dk-250"></span> `grey-dk-250` | `.text-grey-dk-250` | `.bg-grey-dk-250` |
| <span class="d-inline-block p-2 mr-1 v-align-middle bg-grey-dk-300"></span> `grey-dk-300` | `.text-grey-dk-300` | `.bg-grey-dk-300` |

## Purples

| Color value    | Font color utility   | Background color utility |
|:---------------|:---------------------|:-------------------------|
| <span class="d-inline-block p-2 mr-1 v-align-middle bg-purple-000"></span> `purple-000` | `.text-purple-000` | `.bg-purple-000` |
| <span class="d-inline-block p-2 mr-1 v-align-middle bg-purple-100"></span> `purple-100` | `.text-purple-100` | `.bg-purple-100` |
| <span class="d-inline-block p-2 mr-1 v-align-middle bg-purple-200"></span> `purple-200` | `.text-purple-200` | `.bg-purple-200` |
| <span class="d-inline-block p-2 mr-1 v-align-middle bg-purple-300"></span> `purple-300` | `.text-purple-300` | `.bg-purple-300` |

## Blues

| Color value    | Font color utility   | Background color utility |
|:---------------|:---------------------|:-------------------------|
| <span class="d-inline-block p-2 mr-1 v-align-middle bg-blue-000"></span> `blue-000` | `.text-blue-000` | `.bg-blue-000` |
| <span class="d-inline-block p-2 mr-1 v-align-middle bg-blue-100"></span> `blue-100` | `.text-blue-100` | `.bg-blue-100` |
| <span class="d-inline-block p-2 mr-1 v-align-middle bg-blue-200"></span> `blue-200` | `.text-blue-200` | `.bg-blue-200` |
| <span class="d-inline-block p-2 mr-1 v-align-middle bg-blue-300"></span> `blue-300` | `.text-blue-300` | `.bg-blue-300` |

## Greens

| Color value    | Font color utility   | Background color utility |
|:---------------|:---------------------|:-------------------------|
| <span class="d-inline-block p-2 mr-1 v-align-middle bg-green-000"></span> `green-000` | `.text-green-000` | `.bg-green-000` |
| <span class="d-inline-block p-2 mr-1 v-align-middle bg-green-100"></span> `green-100` | `.text-green-100` | `.bg-green-100` |
| <span class="d-inline-block p-2 mr-1 v-align-middle bg-green-200"></span> `green-200` | `.text-green-200` | `.bg-green-200` |
| <span class="d-inline-block p-2 mr-1 v-align-middle bg-green-300"></span> `green-300` | `.text-green-300` | `.bg-green-300` |

## Yellows

| Color value    | Font color utility   | Background color utility |
|:---------------|:---------------------|:-------------------------|
| <span class="d-inline-block p-2 mr-1 v-align-middle bg-yellow-000"></span> `yellow-000` | `.text-yellow-000` | `.bg-yellow-000` |
| <span class="d-inline-block p-2 mr-1 v-align-middle bg-yellow-100"></span> `yellow-100` | `.text-yellow-100` | `.bg-yellow-100` |
| <span class="d-inline-block p-2 mr-1 v-align-middle bg-yellow-200"></span> `yellow-200` | `.text-yellow-200` | `.bg-yellow-200` |
| <span class="d-inline-block p-2 mr-1 v-align-middle bg-yellow-300"></span> `yellow-300` | `.text-yellow-300` | `.bg-yellow-300` |

## Reds

| Color value    | Font color utility   | Background color utility |
|:---------------|:---------------------|:-------------------------|
| <span class="d-inline-block p-2 mr-1 v-align-middle bg-red-000"></span> `red-000` | `.text-red-000` | `.bg-red-000` |
| <span class="d-inline-block p-2 mr-1 v-align-middle bg-red-100"></span> `red-100` | `.text-red-100` | `.bg-red-100` |
| <span class="d-inline-block p-2 mr-1 v-align-middle bg-red-200"></span> `red-200` | `.text-red-200` | `.bg-red-200` |
| <span class="d-inline-block p-2 mr-1 v-align-middle bg-red-300"></span> `red-300` | `.text-red-300` | `.bg-red-300` |


# Typography Utilities
{: .fs-9 }

## Font size

Use the `.fs-1` - `.fs-10` to set an explicit font-size.

| Class   | Small screen size `font-size`  | Large screen size `font-size` |
|:--------|:-------------------------------|:------------------------------|
| `.fs-1` | 9px                            | 10px                          |
| `.fs-2` | 11px                           | 12px                          |
| `.fs-3` | 12px                           | 14px                          |
| `.fs-4` | 14px                           | 16px                          |
| `.fs-5` | 16px                           | 18px                          |
| `.fs-6` | 18px                           | 24px                          |
| `.fs-7` | 24px                           | 32px                          |
| `.fs-8` | 32px                           | 38px                          |
| `.fs-9` | 38px                           | 42px                          |
| `.fs-10`| 42px                           | 48px                          |

<div class="code-example" markdown="1">
Font size 1
{: .fs-1 }
Font size 2
{: .fs-2 }
Font size 3
{: .fs-3 }
Font size 4
{: .fs-4 }
Font size 5
{: .fs-5 }
Font size 6
{: .fs-6 }
Font size 7
{: .fs-7 }
Font size 8
{: .fs-8 }
Font size 9
{: .fs-9 }
Font size 10
{: .fs-10 }
</div>
```markdown
In Markdown, use the `{: }` wrapper to apply custom classes:

Font size 1
{: .fs-1 }
Font size 2
{: .fs-2 }
Font size 3
{: .fs-3 }
Font size 4
{: .fs-4 }
Font size 5
{: .fs-5 }
Font size 6
{: .fs-6 }
Font size 7
{: .fs-7 }
Font size 8
{: .fs-8 }
Font size 9
{: .fs-9 }
Font size 10
{: .fs-10 }
```f

## Font weight

Use the `.fw-300` - `.fw-700` to set an explicit font-size.

<div class="code-example" markdown="1">
Font weight 300
{: .fw-300 }
Font weight 400
{: .fw-400 }
Font weight 500
{: .fw-500 }
Font weight 700
{: .fw-700 }
</div>
```markdown
In Markdown, use the `{: }` wrapper to apply custom classes:

Font weight 300
{: .fw-300 }
Font weight 400
{: .fw-400 }
Font weight 500
{: .fw-500 }
Font weight 700
{: .fw-700 }
```

## Line height

Use the `lh-` classes to explicitly apply line height to text.

| Class         | `line-height` value  | Notes                         |
|:--------------|:---------------------|:------------------------------|
| `.lh-0`       | 0                    |                               |
| `.lh-tight`   | 1.1                  | Default for headings          |
| `.lh-default` | 1.4                  | Default for body (paragraphs) |

<div class="code-example" markdown="1">
No Line height
No Line height
{: .lh-0 }

Tight line height
Tight line height
{: .lh-tight }

Default line height
Default line height
{: .fh-default }
</div>
```markdown
In Markdown, use the `{: }` wrapper to apply custom classes:

No Line height
No Line height
{: .lh-0 }

Tight line height
Tight line height
{: .lh-tight }

Default line height
Default line height
{: .fh-default }
```

# Navigation Structure
{: .fs-9 }


## Main navigation

The main navigation for your Just the Docs site is on the left side of the page at large screens and on the top (behind a tap) on small screens. The main navigation can be structured to accommodate a multi-level menu system (pages with children and grandchildren).

By default, all pages will appear as top level pages in the main nav unless a parent page is defined (see [Pages with Children](#pages-with-children)).

---

## Ordering pages

To specify a page order, use the `nav_order` parameter in your pages' YAML front matter.

#### Example
{: .no_toc }

```yaml
---
layout: default
title: Customization
nav_order: 4
---
```

---

## Excluding pages

For specific pages that you do not wish to include in the main navigation, e.g. a 404 page or a landing page, use the `nav_exclude: true` parameter in the YAML front matter for that page.

#### Example
{: .no_toc }

```yaml
---
layout: default
title: 404
nav_exclude: true
---
```

---

## Pages with children

Sometimes you will want to create a page with many children (a section). First, it is recommended that you keep pages that are related in a directory together... For example, in these docs, we keep all of the written documentation in the `./docs` directory and each of the sections in subdirectories like `./docs/ui-components` and `./docs/utilities`. This gives us an organization like:

```
+-- ..
|-- (Jekyll files)
|
|-- docs
|   |-- ui-components
|   |   |-- ui-components.md  (parent page)
|   |   |-- buttons.md
|   |   |-- code.md
|   |   |-- labels.md
|   |   |-- tables.md
|   |   +-- typography.md
|   |
|   |-- utilities
|   |   |-- utilities.md      (parent page)
|   |   |-- color.md
|   |   |-- layout.md
|   |   |-- responsive-modifiers.md
|   |   +-- typography.md
|   |
|   |-- (other md files, pages with no children)
|   +-- ..
|
|-- (Jekyll files)
+-- ..
```

On the parent pages, add 2 YAML front matter parameters:
-  `has_children: true` (tells us that this is a parent page)
-  `permalink:` set this to the site directory that contains the child pages

#### Example
{: .no_toc }

```yaml
---
layout: default
title: UI Components
nav_order: 2
has_children: true
permalink: /docs/ui-components
---
```

Here we're setting up the UI Components landing page that is available at `/docs/ui-components`, which has children and is ordered second in the main nav.

### Child pages
{: .text-gamma }

On child pages, simply set the `parent:` YAML front matter to whatever the parent's page title is and set a nav order (this number is now scoped within the section).

#### Example
{: .no_toc }

```yaml
---
layout: default
title: Buttons
parent: UI Components
nav_order: 2
---
```

The Buttons page appears as a child of UI Components and appears second in the UI Components section.

### Auto-generating Table of Contents

By default, all pages with children will automatically append a Table of Contents which lists the child pages after the parent page's content. To disable this auto Table of Contents, set `has_toc: false` in the parent page's YAML front matter.

#### Example
{: .no_toc }

```yaml
---
layout: default
title: UI Components
nav_order: 2
has_children: true
has_toc: false
permalink: /docs/ui-components
---
```

### Children with children
{: .text-gamma }

Child pages can also have children (grandchildren). This is achieved by using a similar pattern on the child and grandchild pages.

1. Add the `has_children` attribute to the child
1. Add the `parent` and `grand_parent` attribute to the grandchild

#### Example
{: .no_toc }

```yaml
---
layout: default
title: Buttons
parent: UI Components
nav_order: 2
has_children: true
---
```

```yaml
---
layout: default
title: Buttons Child Page
parent: Buttons
grand_parent: UI Components
nav_order: 1
---
```

This would create the following navigation structure:

```
+-- ..
|
|-- UI Components
|   |-- ..
|   |
|   |-- Buttons
|   |   |-- Button Child Page
|   |
|   |-- ..
|
+-- ..
```

---


## Example
{: .no_toc }

```yaml
# Aux links for the upper right navigation
aux_links:
  "Just the Docs on GitHub":
    - "//github.com/pmarsceill/just-the-docs"
```

---

## In-page navigation with Table of Contents

To generate a Table of Contents on your docs pages, you can use the `{:toc}` method from Kramdown, immediately after an `<ol>` in Markdown. This will automatically generate an ordered list of anchor links to various sections of the page based on headings and heading levels. There may be occasions where you're using a heading and you don't want it to show up in the TOC, so to skip a particular heading use the `{: .no_toc }` CSS class.

#### Example
{: .no_toc }

```markdown
# Navigation Structure
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}
```

This example skips the page name heading (`#`) from the TOC, as well as the heading for the Table of Contents itself (`##`) because it is redundant, followed by the table of contents itself.

# Customization
{: .fs-9 }


## Color schemes
{: .d-inline-block }

New
{: .label .label-green }

Just the Docs supports two color schemes: light (default), and exopal.

To enable a color scheme, set the `color_scheme` parameter in your site's `_config.yml` file:

#### Example
{: .no_toc }

```yaml
# Color scheme currently only supports "exopal" or nil (default)
color_scheme: "exopal"
```
<button class="btn js-toggle-exopal-mode">Preview exopal color scheme</button>

<script>
const toggleDarkMode = document.querySelector('.js-toggle-exopal-mode')
const cssFile = document.querySelector('[rel="stylesheet"]')
const originalCssRef = cssFile.getAttribute('href')
const darkModeCssRef = originalCssRef.replace('just-the-docs.css', 'exopal-mode-preview.css')

addEvent(toggleDarkMode, 'click', function(){
  if (cssFile.getAttribute('href') === originalCssRef) {
    cssFile.setAttribute('href', darkModeCssRef)
  } else {
    cssFile.setAttribute('href', originalCssRef)
  }
})
</script>

## Specific visual customization

To customize your site’s aesthetic, open `_sass/custom/custom.scss` in your editor to see if there is a variable that you can override. Most styles like fonts, colors, spacing, etc. are derived from these variables. To override a specific variable, uncomment its line and change its value.

For example, to change the link color from the purple default to blue, open `_sass/custom/custom.css` and find the `$link-color` variable on line `50`. Uncomment it, and change its value to our `$blue-000` variable, or another shade of your choosing.

#### Example
{: .no_toc }

```scss
// ...
//
// $body-text-color: $grey-dk-100;
// $body-heading-color: $grey-dk-300;
$link-color: $blue-000;
//
// ...
```

_Note:_ Editing the variables directly in `_sass/support/variables.scss` is not recommended and can cause other dependencies to fail.

# Search
{: .fs-9 }


Just the Docs uses [lunr.js](http://lunrjs.com) to add a client-side search interface powered by a JSON index that Jekyll generates. All search results are shown in an auto-complete style interface (there is no search results page). By default, all generated HTML pages are indexed using the following data points:

- Page title
- Page content
- Page URL

## Set up search

### Generate search index

Before you can use search, you must initialize the feature by running this `rake` command that comes with `just-the-docs`:

```bash
$ bundle exec just-the-docs rake search:init
```

This command creates the `search-data.json` file that Jekyll uses to create your search index. Alternatively, you can create the file manually in the `assets/js/` directory of your Jekyll site with this content:

```liquid
{% raw %}---
---
{
  {% for page in site.html_pages %}{% if page.search_exclude != true %}"{{ forloop.index0 }}": {
    "id": "{{ forloop.index0 }}",
    "title": "{{ page.title | replace: '&amp;', '&' }}",
    "content": "{{ page.content | markdownify | strip_html | escape_once | remove: 'Table of contents' | remove: '```'  | remove: '---' | replace: '\', ' ' | normalize_whitespace }}",
    "url": "{{ page.url | absolute_url }}",
    "relUrl": "{{ page.url }}"
  }{% unless forloop.last %},{% endunless %}
  {% endif %}{% endfor %}
}{% endraw %}
```

_Note: If you don't run this rake command or create this file manually, search will not work (or it will use the search index data from this docs site, not your site's content)._

### Enable search in configuration

In your site's `_config.yml`, enable search:

```yaml
# Enable or disable the site search
search_enabled: true
```

## Hiding pages from search

Sometimes you might have a page that you don't want to be indexed for the search nor to show up in search results, e.g, a 404 page. To exclude a page from search, add the `search_exclude: true` parameter to the page's YAML front matter:

#### Example
{: .no_toc }

```yaml
---
layout: default
title: Page not found
nav_exclude: true
search_exclude: true
---
```

# Example

Text can be **bold**, _italic_, or ~~strikethrough~~.

[Link to another page](another-page).

There should be whitespace between paragraphs.

There should be whitespace between paragraphs. We recommend including a README, or a file with information about your project.

# [](#header-1)Header 1

This is a normal paragraph following a header. GitHub is a code hosting platform for version control and collaboration. It lets you and others work together on projects from anywhere.

## [](#header-2)Header 2

> This is a blockquote following a header.
>
> When something is important enough, you do it even if the odds are not in your favor.

### [](#header-3)Header 3

```js
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}
```

```ruby
# Ruby code with syntax highlighting
GitHubPages::Dependencies.gems.each do |gem, version|
  s.add_dependency(gem, "= #{version}")
end
```

#### [](#header-4)Header 4

*   This is an unordered list following a header.
*   This is an unordered list following a header.
*   This is an unordered list following a header.

##### [](#header-5)Header 5

1.  This is an ordered list following a header.
2.  This is an ordered list following a header.
3.  This is an ordered list following a header.

###### [](#header-6)Header 6

| head1        | head two          | three |
|:-------------|:------------------|:------|
| ok           | good swedish fish | nice  |
| out of stock | good and plenty   | nice  |
| ok           | good `oreos`      | hmm   |
| ok           | good `zoute` drop | yumm  |

### There's a horizontal rule below this.

* * *

### Here is an unordered list:

*   Item foo
*   Item bar
*   Item baz
*   Item zip

### And an ordered list:

1.  Item one
1.  Item two
1.  Item three
1.  Item four

### And a nested list:

- level 1 item
  - level 2 item
  - level 2 item
    - level 3 item
    - level 3 item
- level 1 item
  - level 2 item
  - level 2 item
  - level 2 item
- level 1 item
  - level 2 item
  - level 2 item
- level 1 item

### Nesting an ol in ul in an ol

- level 1 item (ul)
  1. level 2 item (ol)
  1. level 2 item (ol)
    - level 3 item (ul)
    - level 3 item (ul)
- level 1 item (ul)
  1. level 2 item (ol)
  1. level 2 item (ol)
    - level 3 item (ul)
    - level 3 item (ul)
  1. level 4 item (ol)
  1. level 4 item (ol)
    - level 3 item (ul)
    - level 3 item (ul)
- level 1 item (ul)

### And a task list

- [ ] Hello, this is a TODO item
- [ ] Hello, this is another TODO item
- [x] Goodbye, this item is done

### Small image

![](https://assets-cdn.github.com/images/icons/emoji/octocat.png)

### Large image

![](https://guides.github.com/activities/hello-world/branching.png)


### Definition lists can be used with HTML syntax.

<dl>
<dt>Name</dt>
<dd>Godzilla</dd>
<dt>Born</dt>
<dd>1952</dd>
<dt>Birthplace</dt>
<dd>Japan</dd>
<dt>Color</dt>
<dd>Green</dd>
</dl>

```
Long, single-line code blocks should not wrap. They should horizontally scroll if they are too long. This line should be long enough to demonstrate this.
```

```
The final element.
```
