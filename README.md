# bulma-helper-spacing

A simple spacing helper to use with Bulma !

It provides spacing utilities using **margin** and **padding** like 
[Bootstrap](https://getbootstrap.com/) does.

## Dependency

You must use [Bulma](https://bulma.io/) as a dependency. 

```
$ npm i --save-dev bulma
```

Be sure to include `base/_all.sass` or at least `utilities/mixins.sass` 
(because spacing is generated with breakpoints for :

* `tablet`
* `desktop`
* `fullhd`

```
@charset "utf-8";

// Import only what you need from Bulma

@import "../../node_modules/bulma/sass/utilities/mixins.sass";
//@import "../../node_modules/bulma/sass/base/_all.sass";
// ...

@import "./spacing.sass";
```

## How-to

Use these classes to generate spacing for *margins* and *paddings*. All 
generated *CSS classes* are using Bulma's **nomenclature**.

```
<div class="has-padding-left-0">
<div class="has-padding-5">
<div class="has-margin-y-3">
<div class="has-padding-x-0 has-padding-top-8-desktop">
<div class="has-margin-5 has-margin-0-desktop">
```


