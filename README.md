# CSS - TLDR;

<p align="center">
<img align="center" alt="CSS" width="96px" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/css/css.png" />
</p>

<p align="center">	
Made as a personal project to gather and organize concepts for learning.
</p>

## Table of Contents

0. ## **[Common properties](#0-fundamentals)**
    + 0.1 **[🟢 Font, text & list properties](#01-font-text---list-properties)**
    + 0.2 **[🟢 Background](#02-consolelog)**
    + 0.3 **[🟢 Margin & padding (Box model)](#03-variables)**
    + 0.4 **[🟢 Positioning](#04-variable-declarations---const--let--var)**
    + 0.5 **[🟢 Border](#05-operators-assignment--comparison--logical--unary)**
    + 0.6 **[🟢 Height & width](#06--vs--vs--assignment--equality)**
    + 0.7 **[🟢 Float](#07-typeof-operator)**
    + 0.8 **[🟡 Display](#08-type-conversion)**
    + 0.9 **[🔴 Flexbox & grid](#09-template-literals---name)**
 
 
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


## 0.1 Font, text & list properties

`color` - #RRGGBB (Red, Green, Blue hex values)

`font-size` - 

`font-style` - 	normal | italic | oblique

`font-weight` - normal | bold | 100 | 400 | 700

`font-family` - 

`text-align` - 	left | right | center | justify

`text-decoration` - none | underline | overline | line-through | blink | inherit

`text-transformation` - none | capitalize | uppercase | lowercase

`list-style` -

`line-height` -

`letter-spacing` - 

`cursor` - 

## Background

`background` - The background property is a shorthand property for other properties:

```css
body {
  background: lightblue url("img_tree.gif") no-repeat fixed center;
}

```

---

`background-color` - #RRGGBB (Red, Green, Blue hex values)

`background-image` - url("[image url]")

`background-repeat` - 	repeat | repeat-x | repeat-y | no-repeat

`background-position` - left | center | right | top | center | bottom

background-size

background-origin

background-clip

background-attachment



## Margin & padding (Box model)

![](https://zellwk.com/images/2013/05/box-model.jpg)

`margin` - 

`padding` - 

```css
div {
    margin-top: 20px;
    margin-bottom: 20px;
    margin-right: 10px;
    margin-left: 10px
}
```

## Positioning

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

## Border

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





## Height & width

`height` & `width` - 

`top` `right` `bottom` `left` - 

```css
img {
    max-width: 100%;
    height: auto;
}
```

## Float


`float` - left right none




## Display

`display` - 








---
