---
layout: default
title: Lists
parent: UI Components
nav_order: 5
---

# Lists
{: .no_toc }

## Table des matière
{: .no_toc .text-delta }

1. TOC
{:toc}

---

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

