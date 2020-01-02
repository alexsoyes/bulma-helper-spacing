<img src="https://raw.githubusercontent.com/jgthms/bulma/master/docs/images/bulma-banner.png" alt="Bulma's logo" width="350" />

A simple spacing helper to use with [Bulma](https://bulma.io/)! It provides spacing utilities using **margin** and **padding** like 
[Bootstrap](https://getbootstrap.com/docs/4.4/utilities/spacing/) does.

In order to work, `bulma-helper-spacing` is using `rem` for sizing. `margin-1` will be equivalent to `margin: 1rem;`

## Prerequisites

You must use [Bulma](https://bulma.io/) as a dependency. 

```
$ npm install bulma
```

*Attention* : Be sure to include `base/_all.sass` or at least `utilities/mixins.sass` and `*-variables.sass`
(because spacing is generated with the following breakpoints taken from Bulma) :

* `tablet`
* `desktop`
* `fullhd`

## Installation

### Available on NPM

```
$ npm install bulma-helper-spacing
```

## Usage

```
// Import only what you need from Bulma
@import './node_modules/bulma/sass/utilities/initial-variables.sass'; // required
@import './node_modules/bulma/sass/utilities/derived-variables.sass'; // required
@import './node_modules/bulma/sass/utilities/mixins'; // required
// @import "../../node_modules/bulma/sass/base/_all.sass"; // avoid including everything from Bulma, we should use its modularity ;-)

// Bulma spacing helper
@import "../../node_modules/bulma-helper-spacing/spacing";

// Do your magic here :)
```

## Documentation

Use these classes to generate spacing for *margins* and *paddings*. All 
generated *CSS classes* are using Bulma's writing style.

```
has-{property}-{sides}(-{size})(-{breakpoint})
```

* Property : `margin`, `padding`
* Sides (optional) : ` `, `x`, `y`, `top`, `bottom`, `left`, `right`
* Size : `0`, `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`
* Breakpoint (optional) : ` `, `tablet`, `desktop`, `fullhd`

### Examples

```
<!-- Padding -->
<div class="has-padding-left-0"></div>
<div class="has-padding-5"></div>
<div class="has-padding-x-0 has-padding-top-8-desktop"></div>

<!-- Margin -->
<div class="has-margin-y-3"></div>
<div class="has-margin-5 has-margin-0-desktop"></div>
```
