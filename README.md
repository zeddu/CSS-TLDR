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
    + 0.8 **[🟡 Float](#08-float)**
    + 0.9 **[🔴 Display](#09-display)**
 
 
 1. ## **[Flexbox](#1-Strings)**
    + 1.1 **[🟢 length / charAt / charCodeAt](#11-length--charat--charcodeat)**
    + 1.2 **[🟢 concat / split / repeat](#12-concat--split--repeat)**
    + 1.3 **[🟢 search / replace](#13-search--replace)**
    + 1.4 **[🟢 slice / substring / substr](#14-slice--substring--substr)**
    + 1.5 **[🟢 toUpperCase / toLowerCase](#15-touppercase--tolowercase)**
    + 1.6 **[🟢 indexOf / lastIndexOf](#16-indexof--lastindexof)**
    + 1.7 **[🟢 trim / padStart / padEnd](#17-trim--padstart--padend)**
    + 1.8 **[🟢 startsWith / endsWith / includes](#18-startswith--endswith--includes)**
    + 1.9 **[🟡 Chaining methods](#19-chaining-methods)**

2. ## **[Grid](#2-control-flow)**
    + 2.1 **[🟢 For loops (for/for in/for of/forEach/backwards for)](#21-for-loops-forfor-infor-offoreachbackwards-for)**
    + 2.2 **[🟢 While loops (while & do-while)](#22-while-loops-while--do-while)**
    + 2.3 **[🟢 If else statement (conditionals)](#23-if-else-statement-conditionals)**
    + 2.4 **[🟡 Ternary if statements (conditionals)](#24-ternary-if-statements-conditionals)**
    + 2.5 **[🟢 Return (conditionals)](#25-return-conditionals)**
    + 2.6 **[🟢 Break (conditionals)](#26-break-conditionals)**
    + 2.7 **[🟢 Continue (conditionals)](#27-continue-conditionals)**
    + 2.8 **[🟢 Break vs continue vs return (conditionals)](#28-break-vs-continue-vs-return-conditionals)**
    + 2.9 **[🟡 Switch statements (conditionals)](#29-switch-statements-conditionals)**


3. ## **[Templates](#3-Functions)**
    + 3.1 **[🟢 Higher order functions & first class citizenship](#31-higher-order-functions---first-class-citizenship)**
    + 3.2 **[🟢 Function declarations (traditional functions)](#32-function-declarations-traditional-functions)**
    + 3.3 **[🟢 Function expressions](#33-function-expressions)**
    + 3.4 **[🟢 Arrow functions & concise arrow functions](#34-arrow-functions--concise-arrow-functions)**
    + 3.5 **[🟢 Anonymous functions](#35-anonymous-functions)**
    + 3.6 **[🟡 Immediately invoked function expressions (IIFE)](#36-immediately-invoked-function-expressions-iife)**
    + 3.7 **[🟡 Recursive functions](#37-recursive-functions)**
    + 3.8 **[🔴 Callback functions](#38-callback-functions)**
    + 3.9 **[🔴 Asynchronous functions](#39-asynchronous-functions)**

**[⬆ Back to Top](#table-of-contents)**


# 0 Common properties 

![](https://i.imgur.com/iqcONqI.png)

---

The goal of a reset stylesheet is to reduce browser inconsistencies in things like default line heights, margins and font sizes of headings, and so on.

📜 - https://meyerweb.com/eric/tools/css/reset/

**[⬆ Back to Top](#common-properties)**


## 0.1 Font & text properties

`color` - #RRGGBB (Red, Green, Blue hex values)

`font-size` - px | em | rem

`font-style` - 	normal | italic | oblique

`font-weight` - normal | bold | 100 | 400 | 700

`font-family` - "Roboto", sans-serif

`text-align` - 	left | right | center | justify

`text-decoration` - none | underline | overline | line-through | blink | inherit

`text-transformation` - none | capitalize | uppercase | lowercase

`list-style` - none | list-style-type || list-style-position || list-style-image

`line-height` - px etc.

`letter-spacing` - px etc.

`cursor` - pointer | grabbing | copy | crosshair | many more..

**[⬆ Back to Top](#common-properties)**

## 0.2 Background

📜 - https://bitsofco.de/the-background-properties/

---

`background` - The background property is a shorthand property for other properties:

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

---



![](https://css-tricks.com/wp-content/uploads/2015/02/cover-and-contain.jpg)



**[⬆ Back to Top](#common-properties)**


## 0.3 Margin & padding (Box model)

![](https://zellwk.com/images/2013/05/box-model.jpg)

`margin` - px | em | rem | % | auto | initial | inherit

`padding` - px | em | rem | % | auto | initial | inherit

```css
div {
    margin-top: 20px;
    margin-bottom: 20px;
    margin-right: 10px;
    margin-left: 10px
}
```

**[⬆ Back to Top](#common-properties)**


## 0.4 Positioning

> ![](https://www.webideasole.com/wp-content/uploads/2019/02/css_positions-1024x349.png)
> Static, relative & absolute

`top` `right` `bottom` `left` - auto | px/em/rem | % | initial | inherit

`position` - static | absolute | fixed | relative | sticky | initial | inherit

- static - Default value. Elements render in order, as they appear in the document flow

- absolute - The element is positioned relative to its first positioned (not static) ancestor element

- fixed	- The element is positioned relative to the browser window

- relative - The element is positioned relative to its normal position, so "left:20px" adds 20 pixels to the element's LEFT position

- sticky - The element is positioned based on the user's scroll position. A sticky element toggles between relative and fixed, depending on the scroll position. 

- initial - Sets this property to its default value.

- inherit - Inherits this property from its parent element.

**[⬆ Back to Top](#common-properties)**


## 0.5 Border

![](https://s3.amazonaws.com/webucator-how-tos/2304.png)

`border` - 

```css
div {
    border: 1px solid black;
    /* border width, style and color */
}
```

The border property is a shorthand property for:

`border-width`

`border-style` (required)

`border-color`

**[⬆ Back to Top](#common-properties)**



## 0.6 Height & width

![](https://blogs.igalia.com/mrego/files/2018/08/percent-definite-size.svg)

`width` & `height` - px | %

`min-width` & `min-height` - Defines the minimum width/height of an element

`top` `right` `bottom` `left` - px | %

```css
img {
    max-width: 100%;
    height: auto;
}
```

**[⬆ Back to Top](#common-properties)**


## 0.7 Columns

`columns` - auto | column-width column-count | initial | inherit

![](https://ishadeed.com/assets/uncommon-css/column-rule.png)

---

The columns property is a shorthand property for:

- column-width

- column-count

The column-gap property specifies the gap between the columns.

```cs
div {
  column-gap: 40px;
}
```


**[⬆ Back to Top](#common-properties)**


## 0.8 Float

`float` - none | left | right | initial | inherit

`clear` - none | left | right | both | initial | inherit

![](https://cdn-images-1.medium.com/fit/t/1600/480/1*CFwJ6lMQMOi4Oy7L8Mn17g.png)

---

- The CSS `float` property specifies how an element should float.

- The CSS `clear` property specifies what elements can float beside the cleared element and on which side.

    - none - Allows floating elements on both sides. This is default
    - left - No floating elements allowed on the left side
    - right- No floating elements allowed on the right side
    - both - No floating elements allowed on either the left or the right side
    - inherit - The element inherits the clear value of its parent

📜 - https://www.w3schools.com/howto/howto_css_clearfix.asp



**[⬆ Back to Top](#common-properties)**


## 0.9 Display

`display` - none | inline | block | inline-block | flex | grid

![](https://lh3.googleusercontent.com/proxy/8lKSOEuv4rfXhi2bsgF2N_uSnhyKWItzVwcZDEji4NiDTZ-nX3OAgdg6g6dz_k7odYqt-TnJArJ-abIT0t3Lsw32Myq97VFzJrJZsGRp5Nifz6oQJmd0qZ-KRzhEiKafidTJtPJ_ZjpLDxxgXAhegrvRSfAi)

![](https://miro.medium.com/max/871/1*kI78qZQjw_ax1kJo4lPOcw.png)



```css
div {
    display: block;
    display: inline-block;
    display: inline;
    display: flex;
    display: grid;
    display: none;
}
```

**[⬆ Back to Top](#common-properties)**

---

# 1 Flexbox

📜 - https://css-tricks.com/snippets/css/a-guide-to-flexbox/

```css
display: flex;
```

![](https://darekkay.com/assets/images/covers/flexbox-cheatsheet.png)

---

The goal of a reset stylesheet is to reduce browser inconsistencies in things like default line heights, margins and font sizes of headings, and so on.



**[⬆ Back to Top](#common-properties)**
