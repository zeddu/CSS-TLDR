# CSS - TLDR;

<p align="center">
<img align="center" alt="CSS" width="96px" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/css/css.png" />
</p>

<p align="center">	
Made as a personal project to gather and organize concepts for learning.
</p>

## Table of Contents

0. ## **[Common properties](#0-common-properties)**
    + 0.1 **[🟢 Font & text properties](#01-font--text-properties)**
    + 0.2 **[🟢 Background](#02-background)**
    + 0.3 **[🟢 Margin & padding (Box model)](#03-margin--padding-box-model)**
    + 0.4 **[🟢 Positioning](#04-positioning)**
    + 0.5 **[🟢 Border](#05-border)**
    + 0.6 **[🟢 Height & width](#06-height--width)**
    + 0.7 **[🟢 Columns](#07-Columns)**
    + 0.8 **[🟢 Float](#08-float)**
    + 0.9 **[🟢 Display](#09-display)**
 
 
 1. ## **[Flexbox](#1-flexbox)**
    + 1.1 **[🟢 Basics & terminology](#11-basics--terminology)**
    + 1.2 **[🟢 Flex-direction](#12-flex-direction)**
    + 1.3 **[🟢 Justify-content](#13-justify-content)**
    + 1.4 **[🟢 Align-items](#14-align-items)**
    + 1.5 **[🟢 Flex-wrap](#15-flex-wrap)**
    + 1.6 **[🟢 Flex-flow](#16-flex--flow)**
    + 1.7 **[🟢 Align-content](#17-align-content)**
    + 1.8 **[🟢 Order](#18-order)**
    + 1.9 **[🟢 Flex-grow](#19-flex-grow)**
    + 1.10 **[🟢 Flex-shrink](#110-flex-shrink)**
    + 1.11 **[🟢 Flex-basis](#111-flex-basis)**
    + 1.12 **[🟢 Align-self](#112-align-self)**
    + 1.13 **[🟢 Flex](#113-flex)**
    + 1.14 **[🟢 Flex overview](#114-flex-overview)**

2. ## **[Grid](#2-grid)**
    + 2.1 **[🟢 Grid display](#21-grid-display)**
    + 2.2 **[🟢 Grid container properties](#22-grid-container-properties)**
    + 2.3 **[🟢 Grid gap properties](#23-grid-gap-properties)**
    + 2.4 **[🟢 Grid alignment properties](#24-grid-alignment-properties)**
    + 2.5 **[🟢 Grid items properties](#25-grid-items-properties)**
    + 2.6 **[🟢 Grid items alignment properties](#26-grid-items-alignment-properties)**
    + 2.7 **[🟢 Fluid columns snippet](#27-fluid-columns-snippet)**
    + 2.8 **[🟢 Layouts](#28-layouts)**
    + 2.9 **[🟢 Grid overview & layouts](#29-grid-overview--layouts)**


**[⬆ Back to Top](#table-of-contents)**

---

# 0 Tools

📜 - https://meyerweb.com/eric/tools/css/reset/ (CSS Reset)

📜 - https://necolas.github.io/normalize.css/ (CSS Normalize)

📜 - https://type-scale.com/ (Typescale)

📜 - https://bennettfeely.com/clippy (Clipping)

📜 - https://responsivebreakpoints.com/ (Generate image breakpoints)

📜 - https://svgbackgrounds.com/ (SVG's)

📜 - https://1linelayouts.glitch.me/ (Grid layouts)

📜 - https://codepen.io/WebDevSimplified/pen/BaNMMdN (CSS Tooltip)

📜 - https://grid.malven.co/ (Grid cheat sheet)

📜 - https://flexbox.malven.co/ (Flexbox cheat sheet)


📜 - https://codepen.io/chriscoyier/pen/xBmYJN (Fluid grid layout)

📜 - https://bitsofco.de/the-background-properties/ (Background properties)

---



**[⬆ Back to Top](#common-properties)**


# 1 Syntax


## Background & images



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

![](https://css-tricks.com/wp-content/uploads/2015/02/cover-and-contain.jpg)

---



## Visual & display


`columns` - auto | column-width column-count | initial | inherit

The columns property is a shorthand for: column-width & column-count

`float` - none | left | right | initial | inherit

`clear` - none | left | right | both | initial | inherit

📜 - https://www.w3schools.com/howto/howto_css_clearfix.asp (Float clearfix)

`display` - none | inline | block | inline-block | flex | grid

---

**[⬆ Back to Top](#grid)**

## Flexbox

📜 - https://css-tricks.com/snippets/css/a-guide-to-flexbox/


### Parent (Flex Container)

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


### Children (Flex Items)

`order` - integer;

`flex-grow` - number;

`flex-shrink` - number;

`flex-basis` - length | auto;

`flex` - shorthand for grow, shrink, and basis (default: 0 1 auto)

`align-self` - overrides alignment set on parent

---

**[⬆ Back to Top](#grid)**

## Grid

📜 - https://css-tricks.com/snippets/css/complete-guide-grid


### Grid properties - Parent (Grid Container)

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
 .class1 {
 grid-area: header;
}

.wrapper {
 grid-template-columns: 1fr 3fr;
 grid-template-rows: auto;
 grid-template-areas:
 "header header header header"
 "aside . article article";
}
```

---

`grid-auto-columns` & `grid-auto-rows`


Specifies the size of any auto-generated grid tracks (aka implicit grid tracks). Implicit tracks get created when there are more grid items than cells in the grid or when a grid item is placed outside of the explicit grid.

```css
.container {
  grid-auto-columns: 60px;
}
```

`grid-auto-flow`

If you have grid items that you don’t explicitly place on the grid, the auto-placement algorithm kicks in to automatically place the items. This property controls how the auto-placement algorithm works.

```css
.container {
  grid-auto-flow: row | column | row dense | column dense;
}
```

---

`grid` - shorthand for all of the above properties.


A shorthand for setting all of the following properties in a single declaration: grid-template-rows, grid-template-columns, grid-template-areas, grid-auto-rows, grid-auto-columns, and grid-auto-flow 

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

**[⬆ Back to Top](#grid)**

### Grid item properties - Children (Grid items)


`grid-column-start`
`grid-column-end`
`grid-row-start`
`grid-row-end`

Determines a grid item’s location within the grid by referring to specific grid lines. grid-column-start/grid-row-start is the line where the item begins, and grid-column-end/grid-row-end is the line where the item ends.

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

Shorthand for grid-column-start + grid-column-end, and grid-row-start + grid-row-end, respectively.

```css
.item-c {
  grid-column: 3 / span 2;
  grid-row: third-line / 4;
}
```

---

`grid-area`

Gives an item a name so that it can be referenced by a template created with the grid-template-areas property. Alternatively, this property can be used as an even shorter shorthand for grid-row-start + grid-column-start + grid-row-end + grid-column-end.

```css
.item-d {
  grid-area: header;
}
```

---

**[⬆ Back to Top](#grid)**


### Grid alignment properties


`justify-items` - start | end | center | stretch

Aligns grid items along the inline (row) axis (as opposed to align-items which aligns along the block (column) axis). This value applies to all grid items inside the container.

---

`align-items` - start | end | center | stretch

Aligns grid items along the inline (row) axis (as opposed to align-items which aligns along the block (column) axis). This value applies to all grid items inside the container.

---

`place-items` - align-items justify-items

place-items sets both the align-items and justify-items properties in a single declaration.

---

`justify-content` - start | end | center | stretch | space-around | space-between | space-evenly

This property aligns the grid along the inline (row) axis (as opposed to align-content which aligns the grid along the block (column) axis).

---


`align-content` - start | end | center | stretch | space-around | space-between | space-evenly

This property aligns the grid along the block (column) axis (as opposed to justify-content which aligns the grid along the inline (row) axis).

---

`place-content` - align-content justify-content

place-content sets both the align-content and justify-content properties in a single declaration.

---

`align-self` - start | end | center | stretch

---

`justify-self` - start | end | center | stretch


Aligns a grid item inside a cell along the inline (row) axis (as opposed to align-self which aligns along the block (column) axis). This value applies to a grid item inside a single cell.

```css
.item-a {
    justify-self: start;
    justify-self: center;
    justify-self: end;
}
```

---

`place-self` - align-self justify-self

place-self sets both the align-self and justify-self properties in a single declaration.

The first value sets align-self, the second value justify-self. If the second value is omitted, the first value is assigned to both properties.

```css
.item-a {
  place-self: center;
}
```

---

**[⬆ Back to Top](#grid)**







