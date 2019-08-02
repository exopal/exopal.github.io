---
layout: default
title: Code
parent: UI Components
nav_order: 6
---

# Code
{: .no_toc}

## Table des matières
{: .no_toc .text-delta}

1. COT
{: toc}

---

## code en ligne

Le code peut être rendu en ligne en l’enveloppant dans des ticks simples.

<div class = "exemple de code" markdown = "1">
Lorem ipsum dolor sit amet, `<extrait de code en ligne>` élit adipisicing, fait une incursion temporelle dans le travail et dolore magna aliqua.
</ div>
```markdown
Lorem ipsum dolor sit amet, `<extrait de code en ligne>` élit adipisicing, fait une incursion temporelle dans le travail et dolore magna aliqua.
```

---

## Syntax en surbrillance des blocs de code

Utilisez la syntaxe intégrée de Jekyll en mettant en surbrillance Rouge pour les blocs de code en utilisant trois backticks, suivis du nom de la langue:

<div class = "exemple de code" markdown = "1">
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

<div class = "exemple de code" markdown = "1">

<div class = "exemple de code" markdown = "1">

[Bouton de lien](http://example.com/){: .btn}

</div>

```markdown
[Bouton de lien](http://example.com/){: .btn}
```

</div>
{% highlight markdown %}
<div class = "exemple de code" markdown = "1">

[Bouton de lien](http://example.com/) {: .btn}

</div>

```markdown
[Bouton de lien](http://example.com/){: .btn}
```

{% endhighlight %}