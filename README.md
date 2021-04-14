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
 
 
 1. ## **[Flexbox](#1-flexbox)**
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


# 1 Flexbox

📜 - https://css-tricks.com/snippets/css/a-guide-to-flexbox/

```css
.container {
display: flex;
}
```

![](https://darekkay.com/assets/images/covers/flexbox-cheatsheet.png)


**[⬆ Back to Top](#flexbox)**


## 1.1 Basics & terminology

Since `flexbox` is a whole module and not a single property, it involves a lot of things including its whole set of properties. Some of them are meant to be set on the container (parent element, known as “flex container”) whereas the others are meant to be set on the children (said “flex items”).

![](https://css-tricks.com/wp-content/uploads/2018/11/00-basic-terminology.svg)

---

- main axis – The main axis of a flex container is the primary axis along which flex items are laid out. Beware, it is not necessarily horizontal; it depends on the flex-direction property (see below).

- main-start | main-end – The flex items are placed within the container starting from main-start and going to main-end.

- main size – A flex item’s width or height, whichever is in the main dimension, is the item’s main size. The flex item’s main size property is either the ‘width’ or ‘height’ property, whichever is in the main dimension.

- cross axis – The axis perpendicular to the main axis is called the cross axis. Its direction depends on the main axis direction.

- cross-start | cross-end – Flex lines are filled with items and placed into the container starting on the cross-start side of the flex container and going toward the cross-end side.

- cross size – The width or height of a flex item, whichever is in the cross dimension, is the item’s cross size. The cross size property is whichever of ‘width’ or ‘height’ that is in the cross dimension.


**[⬆ Back to Top](#flexbox)**


## 1.1 Flex-direction

 `flex-direction` - row | row-reverse | column | column-reverse

![](https://samanthaming.gumlet.io/flexbox30/9-flex-direction.jpg.gz)

**[⬆ Back to Top](#flexbox)**



## 1.2 Justify-content

`justify-content` - flex-start | flex-end | center | space-between | space-around | space-evenly | start | end | left | right

This defines the alignment along the main axis.

![](https://miro.medium.com/max/434/1*iigDGiNFBOUVJQ_07C1B2g.png)

**[⬆ Back to Top](#flexbox)**


## 1.2 Align-items

`align-items` - stretch | flex-start | flex-end | center | baseline | first baseline | last baseline | start | end

This defines the default behavior for how flex items are laid out along the cross axis on the current line.

![](https://notes.anjagusev.com/static/8a7afe991a11023398a91abddd2567dc/b9e4f/ScreenShot2019-03-22at174821.png)

**[⬆ Back to Top](#flexbox)**

## 1.3 Flex-wrap

`flex-wrap` - nowrap | wrap | wrap-reverse

- `nowrap` (default) - all flex items will be on one line

- `wrap` - flex items will wrap onto multiple lines, from top to bottom.

- `wrap-reverse` - flex items will wrap onto multiple lines from bottom to top.

By default, flex items will all try to fit onto one line. You can change that and allow the items to wrap as needed with this property.

![](https://samanthaming.gumlet.io/flexbox30/10-flex-wrap.jpg.gz)

**[⬆ Back to Top](#flexbox)**


## 1.3 Flex-flow

`flex-flow` - row | row-reverse | column | column-reverse | wrap | nowrap | wrap-reverse

This is a shorthand for the flex-direction and flex-wrap properties, which together define the flex container’s main and cross axes. The default value is row nowrap.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1592610517892/2LRbRRnu_.png)

![](https://miro.medium.com/max/3160/1*xAPNrU9sKijsJnMJOTyUBA.png)

**[⬆ Back to Top](#flexbox)**


## 1.4 Align-content

`align-content` - flex-start | flex-end | center | space-between | space-around | space-evenly | stretch | start | end | baseline

This aligns a flex container’s lines within when there is extra space in the cross-axis, similar to how justify-content aligns individual items within the main-axis.

![](https://on.notist.cloud/slides/deck501/large-30.png)

**[⬆ Back to Top](#flexbox)**


## 1.4 Order

`order` - number

```css
.item {
  order: 5; /* default is 0 */
}
```

By default, flex items are laid out in the source order. However, the order property controls the order in which they appear in the flex container.

![](https://coursesweb.net/addons/css/flexbox-order.jpg)

**[⬆ Back to Top](#flexbox)**


## 1.5 Flex-grow

`flex-grow` - number (this is a relational value)

This defines the ability for a flex item to grow if necessary. It accepts a unitless value that serves as a proportion. It dictates what amount of the available space inside the flex container the item should take up.

If all items have flex-grow set to 1, the remaining space in the container will be distributed equally to all children. If one of the children has a value of 2, the remaining space would take up twice as much space as the others (or it will try to, at least).

![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ8WgTeGfN81LxapVOnt9ufYrzGowZ9PeVmaw&usqp=CAU)

![](https://ishadeed.com/assets/flex-css/flex-grow-1.png)

**[⬆ Back to Top](#flexbox)**


## 1.5 Flex-shrink

`flex-shrink` - number (relational value). Negative numbers are invalid.

This defines the ability for a flex item to shrink if necessary.

![](https://samanthaming.gumlet.io/flexbox30/23-flex-shrink.jpg.gz)

**[⬆ Back to Top](#flexbox)**


## 1.6 Flex-basis

`flex-basis` - 0 | auto

This defines the default size of an element before the remaining space is distributed. It can be a length (e.g. 20%, 5rem, etc.) or a keyword. The auto keyword means “look at my width or height property”.

![](https://www.w3.org/TR/css-flexbox-1/images/rel-vs-abs-flex.svg)

**[⬆ Back to Top](#flexbox)**


## 1.7 Align-self

`align-self` - auto | flex-start | flex-end | center | baseline | stretch

This allows the default alignment (or the one specified by align-items) to be overridden for individual flex items.

![](https://miro.medium.com/max/1072/1*uUfr2oc8xRg4S1YWnRiSDQ.png)

**[⬆ Back to Top](#flexbox)**


## 1.8 Flex

`flex` (Default: 0 1 auto) - none | flex-grow flex-shrink flex-basis

This is the shorthand for flex-grow, flex-shrink and flex-basis combined. The second and third parameters (flex-shrink and flex-basis) are optional. The default is 0 1 auto, but if you set it with a single number value, it’s like 1 0.

It is recommended that you use this shorthand property rather than set the individual properties. The shorthand sets the other values intelligently.

![](https://samanthaming.gumlet.io/flexbox30/27-flex.jpg.gz?format=auto)

**[⬆ Back to Top](#flexbox)**


## 1.9 Flex overview


![](https://samanthaming.gumlet.io/flexbox30/30-flexbox-cheatsheet.jpg.gz?format=auto)

![](https://res.cloudinary.com/practicaldev/image/fetch/s--A8IfWktx--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/prq36s69xfan04a3ah28.png)

**[⬆ Back to Top](#flexbox)**
