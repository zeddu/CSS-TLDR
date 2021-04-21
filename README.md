# CSS - TLDR;

<p align="center">
<img align="center" alt="CSS" width="96px" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/css/css.png" />
</p>

<p align="center">	
Made as a personal project to gather and organize concepts for learning.
</p>

## Table of Contents

0. ## **[Links](#0-Links)**
    + 0.1 **[🟢 CSS Reset](#01-css-reset)**
    + 0.2 **[🟢 Typography](#02-typography)**
    + 0.3 **[🟢 Logos & images](#03-logos--images)**
    + 0.4 **[🟢 CSS components & layouts](#04-css-components--layouts)**
    + 0.5 **[🟢 Tools](#05-tools)**
    + 0.6 **[🟢 Information & guides](#06-information--guides)**
    + 0.7 **[🟢 Snippets](#07-snippets)**
 
0. ## **[Code](#0-Links)**
    + 0.1 **[🟢 CSS Reset](#01-css-reset)**
    + 0.2 **[🟢 Typography](#02-typography)**
    + 0.3 **[🟢 Logos & images](#03-logos--images)**
 
 1. ## **[Syntax](#1-syntax)**
    + 1.1 **[🟢 Background & images](#11-background--images)**
    + 1.2 **[🟢 Visual & display](#12-visual--display)**
    + 1.3 **[🟢 Flex container](#13-flex-container)**
    + 1.4 **[🟢 Flex items](#14-flex-items)**
    + 1.5 **[🟢 Grid container](#15-grid-container)**
    + 1.6 **[🟢 Grid items](#16-grid-items)**
    + 1.7 **[🟢 Grid alignment properties](#17-grid-alignment-properties)**



---

# 0 Links

A list of curated links

### 0.1 CSS Reset

📜 - https://meyerweb.com/eric/tools/css/reset/ (CSS Reset)

📜 - https://necolas.github.io/normalize.css/ (CSS Normalize)

### 0.2 Typography

📜 - https://fonts.google.com/ (Google Fonts)

📜 - https://type-scale.com/ (Typescale)


### 0.3 Logos & images

📜 - https://fontawesome.com/ (Fontawesome)

📜 - https://svgbackgrounds.com/ (SVG's)

📜 - https://responsivebreakpoints.com/ (Generate image breakpoints)



### 0.4 CSS components & layouts

📜 - https://bennettfeely.com/clippy (Clipping tool)

📜 - https://codepen.io/WebDevSimplified/pen/BaNMMdN (CSS Tooltip)

📜 - https://1linelayouts.glitch.me/ (Grid layouts - Google)

📜 - https://codepen.io/chriscoyier/pen/xBmYJN (Fluid grid layout)

📜 - https://philipwalton.github.io/solved-by-flexbox/ (Some layouts)

📜 - https://gridbyexample.com/ (Layouts)


### 0.5 Tools


📜 - https://formspree.io (Formspree forms)


### 0.6 Information & guides

📜 - https://developer.mozilla.org/en-US/docs/Web/CSS/Reference (CSS Syntax list)

📜 - https://bitsofco.de/the-background-properties/ (Background properties)

📜 - https://grid.malven.co/ (Grid cheat sheet)

📜 - https://flexbox.malven.co/ (Flexbox cheat sheet)

📜 - https://css-tricks.com/snippets/css/a-guide-to-flexbox/ (Flexbox guide)

📜 - https://css-tricks.com/snippets/css/complete-guide-grid/ (Grid guide)

📜 - https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout/Basic_Concepts_of_Grid_Layout (MDN Grid basics)

📜 - https://css-tricks.com/collection-interesting-facts-css-grid-layout/ (Interesting Grid facts)

📜 - http://the-echoplex.net/flexyboxes/ (Flex playground & code generator)

📜 - https://www.html5rocks.com/en/tutorials/responsive/picture-element/ (HTML Picture tag)

---

### 0.7 Snippets

#### Fundamentals : 

Color & contrast

Whitespace

Scale

Visual hierarchy

Typohraphy

and all of them consistently

- Good to seperate style rules from layout rules.

- Don't use id's for styling. Specificity. Id's are ok for js hooks.

```css
/** SMACSS
* 01 - Base: applies to HTML, no class/ID selectors
* 02 - Layout: big page sections - .header, .sidebar, etc.
* 03 - Module: encapsulated modeles, re-usable (variables)
* 04 - State: overrides defaults - e.g. is-opened
* 05 - Theme: optional, if theming needed
* 06 - Improve: todo list, shame
**/
```

```css
/** Main
* CH01 - Resets
* CH02 - Globals
* CH03 - Variables
* CH04 - Typography
* CH05 - Page Structure
* CH06 - Header & Navigation
* CH07 - Content * Media
* CH08 - Footer
* CH09 - Miscellaneous
**/
```

```css
/* Initialize box-sizing */
*, *:before, *after {
box-sizing: border-box;
}
```

```css
/* Vanilla CSS imports. Like SASS partials however,
every CSS file will be downloaded at request */
@import url('CSS/reset.css');
@import url('CSS/layout.css');
@import url('CSS/typography.css');
@import url('CSS/masthead.css');
```


```css
/* Center a div */
.parent {
  display: grid;
  place-content: center;
  height: 100vh;
}
```

```css
/* Centering */
div {
width: 80%;
height: 100vh;
background: lightblue;
text-align: center;
margin: 0 0 0 auto;
/* or margin: auto*/
}
```


```scss
/* Whitespace spacing */
.any {
  margin: 10vw;
  padding: 10vw;
}
```

```css
/* Sass mixins - useful background */
@mixin sectionPadding {
padding: 60px 0;
}

@mixin fullImage {
background-size: cover;
background-repeat: no-repeat;
background-position: 0 0;
}

@mixin transition15 {
transition: all 0.15s ease-out 0s;
}
```

**[⬆ Back to Top](#CSS---TLDR)**


# 1 Syntax

📜 - https://developer.mozilla.org/en-US/docs/Web/CSS/Reference

## 1.1 Background & images



```css
body {
  background: lightblue url("img_tree.gif") no-repeat fixed center;
}

```

`background-color` - #RRGGBB (Red, Green, Blue hex values)

`background-image` - url("[image url]")

`background-repeat` - 	repeat | repeat-x | repeat-y | no-repeat

`background-position` - left | center | right | top | center | bottom

`background-size` - auto | contain | cover | % | px

`background-origin` - padding-box | border-box | content-box | initial | inherit

`background-clip` - padding-box | border-box | content-box | initial | inherit

`background-attachment` - scroll | fixed | local | initial | inherit

`width` & `height` - px | %

`min-width` & `min-height` - Defines the minimum width/height of an element

`top` `right` `bottom` `left` - px | %

`object-fit` - fill | contain | cover | scale-down | none | initial | inherit;

`object-position` - x/y coordinates

---

**[⬆ Back to Top](#CSS---TLDR)**

## 1.2 Visual & display


`columns` - auto | column-width column-count | initial | inherit

The columns property is a shorthand for: column-width & column-count

`float` - none | left | right | initial | inherit

`clear` - none | left | right | both | initial | inherit

📜 - https://www.w3schools.com/howto/howto_css_clearfix.asp (Float clearfix)

`display` - none | inline | block | inline-block | flex | grid

---

**[⬆ Back to Top](#CSS---TLDR)**


## 1.3 Flex container

`display` - flex | inline-flex;

`flex-direction` - row | row-reverse | column | column-reverse;

`flex-wrap` - wrap | nowrap | wrap-reverse;

`flex-flow` - (shorthand for flex-direction and flex-wrap)

`justify-content` - (main axis): flex-start | flex-end | center | space-between | space-around |
space-evenly;

`align-items` - (cross axis - adjust to individual sizes): flex-start | flex-end | center | baseline |
stretch;

`align-content` - (cross axis - adjust to largest item): flex-start | flex-end | center | stretch |
space-between | space-around;


## 1.4 Flex items

`order` - integer;

`flex-grow` - number;

`flex-shrink` - number;

`flex-basis` - length | auto;

`flex` - shorthand for grow, shrink, and basis (default: 0 1 auto)

`align-self` - overrides alignment set on parent

---

**[⬆ Back to Top](#CSS---TLDR)**


## 1.5 Grid container

`display` - grid | inline-grid;

---

`grid-template-columns` & `grid-template-rows` - track-size | repeat (track-size: length, %, fr, auto)

```css
 .myClass {
 grid-template-rows: 1fr 2fr 1fr;
 grid-template-columns: 50% 25vh auto;
}
```

`grid-template` - Shorthand for grid-template-rows, grid-template-columns, and grid-template-areas in
1 declaration.

```css
.grid-container {
  display: grid;
  grid-template: 150px / auto auto auto;
}
```


---



`grid-template-areas` -  List of names of areas.

```css
 .item {
 grid-area: header;
}

.grid {
 grid-template-columns: 1fr 3fr;
 grid-template-rows: auto;
 grid-template-areas:
 "header header header header"
 "aside . article article";
}
```

---

`grid-auto-columns` & `grid-auto-rows`

```css
.container {
  grid-auto-columns: 60px;
}
```

`grid-auto-flow`

```css
.container {
  grid-auto-flow: row | column | row dense | column dense;
}
```

---

`grid` - shorthand for all of the above properties.

```css
.container {
  grid: 100px 300px / 3fr 1fr;
}

.container {
  grid-template-rows: 100px 300px;
  grid-template-columns: 3fr 1fr;
}
```


--- 

`grid-gap` or `grid-column-gap` & `grid-row-gap` - gaps

`gap` or `column-gap` & `row-gap` - gaps

--- 

**[⬆ Back to Top](#CSS---TLDR)**

## 1.6 Grid items


`grid-column-start`
`grid-column-end`
`grid-row-start`
`grid-row-end`

```css
.item-a {
  grid-column-start: 2;
  grid-column-end: five;
  grid-row-start: row1-start;
  grid-row-end: 3;
}
```

---

`grid-column` & `grid-row`

```css
.item-c {
  grid-column: 3 / span 2;
  grid-row: third-line / 4;
}
```

---

`grid-area`

```css
.item-d {
  grid-area: header;
}
```

---

**[⬆ Back to Top](#CSS---TLDR)**


## 1.7 Grid alignment properties

`justify-items` - start | end | center | stretch

`align-items` - start | end | center | stretch

`place-items` - align-items justify-items

`justify-content` - start | end | center | stretch | space-around | space-between | space-evenly

`align-content` - start | end | center | stretch | 

`place-content` - align-content justify-content

`align-self` - start | end | center | stretch

`justify-self` - start | end | center | stretch

`place-self` - align-self justify-self

---

**[⬆ Back to Top](#CSS---TLDR)**
