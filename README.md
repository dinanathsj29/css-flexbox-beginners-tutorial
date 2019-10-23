<p align="center">
  <img src="_images-css-flexbox/1-css3-logo-1.png" alt="CSS Flexbox" title="CSS Flexbox" width="200" />
</p>

CSS Flexbox
=====================

CSS Flexible Box Layout Module (Flexbox) is one of the most widely used and popular mechanisms which provides flexibility to create/build or design professional layouts/nested layouts.

Welcome
---------------------

Hi All, I'm **`Dinanath Jayaswal, Senior UI/Web Developer and Adobe Certified Expert Professional`**, I wanna welcome you to CSS Flexbox Tutorial for beginners. 

About the Course/Tutorial
---------------------

This is a comprehensive guide to CSS flexbox layout. This complete guide explains everything about the flexbox.

Who is this for? 
---------------------

This Course/Tutorial is ideal for:
- Any Web designer/developer interested in getting a deep understanding of Flexbox
- CSS lovers
- Candidates desire to become CSS Expert and better Front End web Developer / Designer
- Web designers/developers who want to improve skills with new web standards

Course/Tutorial achievement
---------------------

Course/Tutorial Goal
---------------------

After completing/attending/finishing this Course/Tutorial, participants should be able to: 
- Align elements using modern CSS module, like CSS Flexbox 
  - vertically align any element
- Use the new CSS3 Flexbox box model to create responsive web layouts more effectively!
  - add spacing between elements
  - take up remaining space
- Use/Operate CSS Flexbox confidently to create modern/advanced layouts
  - implement complete site layouts / create modern grids

Prerequisites for current course / What you need to know
---------------------

- Basic knowledge of HTML5 and CSS3

Topics included/covered
=====================

1. [Introduction to CSS Flexbox](#1-introduction-to-css-flexbox)
    - 1.1. [What is CSS Flexbox](#11-what-is-css-flexbox)
    - 1.2. [Layout modes](#12-layout-modes)
    - 1.3. [Why Flexbox?](#13-why-flexbox)
    - 1.4. [Important Terminology](#14-important-terminology)
    - 1.5. [Flexbox axis](#15-flexbox-axis)
    - 1.6. [Browser support](#16-browser-support)

2. [Flex Container Properties](#2-flex-container-properties)
    - 2.1. [Flex Display](#21-flex-display)
    - 2.2. [Flex Direction](#22-flex-direction)
    - 2.3. [Flex Wrap](#23-flex-wrap)
    - 2.4. [Flex Flow](#24-flex-flow)
    - 2.5. [Justify Content](#25-justify-content)
    - 2.6. [Align Items](#26-align-items)

1 Introduction to CSS Flexbox
=====================

1.1. What is CSS Flexbox
---------------------

`CSS Flexible Box Layout Module` is also known and referred to as `CSS Flexbox`, is designed for one-dimensional layout model that makes it easy to:
- Design flexible and efficient layouts
- Distribute space among items
- Control alignments of objects/elements/items in given container
- Flexbox layout is most appropriate to the components of an application, and small-scale layouts
- Flexbox is a new CSS display type designed to craft CSS layouts in a much easier way
- Control the position, size, and spacing of child elements relative to parent container and other child elements
- W3C Candidate Recommendation as of October 2017

1.2. Layout modes
---------------------

Before CSS Flexbox there were 4 layout modes/models:
1. **`Block`** (for different sections in a webpage)
2. **`Inline`** (for text and spans in the same line)
3. **`Table`** (for two-dimensional tabular data)
4. **`Position`** (for the explicit position of an element)

### Pre-Flexbox we have used:
- Different positional properties like `fixed, absolute` to set alignment at the exact required place
- Floats and clear fixes to create navigation, detailed section
- Fixed heights columns to show equality
- Above mentioned layout modes does not provide enough flexibility to create/build or design professional/nested/modern layouts
- we need to include another CSS mechanism like Floats, Vertical alignment of text/elements and other hacks with Margin, Padding to create the accurate/desired layout
- CSS Flexible Box Layout Module (Flexbox), makes it easier to design flexible responsive layout structure without using float or positioning

1.3. Why Flexbox?
---------------------

- Flex/CSS Flexbox layout provides lots of flexibilities while creating complex layouts like:
  - arrange items from left to right or top to bottom and vice versa
  - adjust the spacing between objects
  - alignments of items
  - order and placements of various elements 
  - improve the items alignment, directions and order in the container even when they are with dynamic or even unknown size
  - equal height columns
  - ability to modify the width or height of its children to fill the available space in the best possible way on different screen sizes
  - Flexbox is a new CSS display type designed to craft CSS layouts in a much easier way
  - Control the position, size, and spacing of child elements relative to parent container and other child elements
  - CSS flexbox works great responsively (RWD - Responsive Web Design)
  - Bootstrap 4 is built-on with Flex layout Model

1.4. Important Terminology
---------------------

Let's learn some of the Important Terminology/concepts related to CSS flexbox to get proper understandings and how it works. There are main three terms or entities while dealing with flexbox:
1. **`Flex Container`** (Parent/Container to hold sub-items)
2. **`Flex Items`** (Child/sub-items)
3. **`Flexbox axis`** (Main axis [horizontal] and Cross axis [vertical])

> **Syntax & Example**: `1.4-flex-container-item.html basic markup`

```html
<div class="main-container">
  <div class="item item-1">item-1</div>
  <div class="item item-2">item-2</div>
  <div class="item item-3">item-3</div>
  <div class="item item-4">item-4</div>
  <div class="item item-5">item-5</div>
  <div class="item item-6">item-6</div>
  <div class="item item-7">item-7</div>
  <div class="item item-8">item-8</div>
  <div class="item item-9">item-9</div>
  <div class="item item-10">item-10</div>
</div>
```

<hr/>

> **Syntax & Example**: `1.4-flex-container-item.html default`

```html
<!DOCTYPE html>

<html lang="en">

  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>1.4-flex-container-item.html</title>

    <style type="text/css">

      body {
        margin: 0;
        padding: 0;
        font-family: verdana;
      }

      .main-container {
        border: 4px solid #826a98;
      }

      .item {
        color: #ffffff;
        font-size: 1rem;
        padding: 0.75rem;
        text-align: center;
      }

      .item-1 {
        background-color:#DDA0DD;
      }

      .item-2 {
        background-color:#BF94E4;
      }

      .item-3 {
        background-color:#734F96;
      }

      .item-4 {
        background-color:#FBAED2;
      }

      .item-5 {
        background-color:#EE82EE;
      }
      
      .item-6 {
        background-color:#ADE4CA;
      }

      .item-7 {
        background-color:#A6D5AE;
      }

      .item-8 {
        background-color:#8FBC8E;
      }

      .item-9 {
        background-color: #64A466;
      }
      
      .item-10 {
        background-color:#2E8B56;
      }

    </style>

  </head>

  <body>

    <div class="main-container">
      <div class="item item-1">item-1</div>
      <div class="item item-2">item-2</div>
      <div class="item item-3">item-3</div>
      <div class="item item-4">item-4</div>
      <div class="item item-5">item-5</div>
      <div class="item item-6">item-6</div>
      <div class="item item-7">item-7</div>
      <div class="item item-8">item-8</div>
      <div class="item item-9">item-9</div>
      <div class="item item-10">item-10</div>
    </div>
    
  </body>
  
</html>
```

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/1.4-flex-container-item-1-default.png" alt="Flex parent container and flex child item markup" title="Flex parent container and flex child item markup" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - Flex parent container and flex child item markup </figcaption>
  </figure>
</p>

<hr/>

> **Syntax & Example**: `1.4-flex-container-item.html display:flex`

```html
<style type="text/css">
  .main-container {
    border: 4px solid #826a98;
    display: flex; /* block level flex container */
  }
</style>
```

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/1.4-flex-container-item-2-display-flex.png" alt="Flex parent container, child item with display flex" title="Flex parent container, child item with display flex" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - Flex parent container, child item with display flex </figcaption>
  </figure>
</p>

<hr/>

1.5. Flexbox axis
---------------------

1. **`Main Axis`**
    - By default, main/primary axis runs Left to Right
    - Its denoted with terms like the main start and main end
    - The length between the main start to the main end is known as the main size
2. **`Cross Axis`**
    - By default, cross-axis runs Top to Bottom
    - Its denoted with terms like cross start and cross end
    - The length between cross start to cross end is known as cross size

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/1.5-flex-axis-1.png" alt="flex axis - main axis and cross axis" title="flex axis - main axis and cross axis" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - flex axis - main axis and cross axis </figcaption>
  </figure>
</p>

<hr/>

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/1.5-flex-axis-2.png" alt="flex axis - main axis and cross axis" title="flex axis - main axis and cross axis" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - flex axis - main axis and cross axis </figcaption>
  </figure>
</p>

<hr/>

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/1.5-flex-axis-3-row-column.png" alt="flex axis - main axis and cross axis for Row and Column" title="flex axis - main axis and cross axis for Row and Column" width="400" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - flex axis - main axis and cross axis for Row and Column </figcaption>
  </figure>
</p>

1.6. Browser support
---------------------

The flexbox properties are supported in all modern browsers:

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/1.6-browser-support.png" alt="css flexbox browser support" title="css flexbox browser support" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - css flexbox browser support </figcaption>
  </figure>
</p>

2 Flex Container Properties
===================== 

Let's look into some of the important properties used with Flex Container:
- **`display`**
  - It defines the Flex Container inline or block
  - An important and mandatory property to work with Flexbox
- **`flex-direction`**
  - Defines direction for flex items to be placed inside Flex Container
- **`flex-wrap`**
  - Set wrapping of items within Flex Container (overflow item placement)
- **`flex-flow`**
  - Short-hand property for a combination of flex-direction and flex-wrap
- **`justify-content`**
  - Defines alignment of items along the main axis
- **`align-items`**
  - How flex items layout/laid out with the cross axis
- **`align-content`**
  - Alignment of items along the cross axis (if multiple rows/lines available)


2.1. Flex Display
---------------------

- To create a flex container, we set the value of the container's `display` property to `flex` or `inline-flex`
- It enables a flex context for all its direct children

`display` property creates either a `block-level` or `inline-level` flex container:
- **`display: flex`**;
  - block level flex, covers 100% width
- **`display: inline-flex`**;
  - inline-level, same line flex, covers only required width as per items width
- syntax:
```css 
.container {
  /* display: flex; */ /* block level flex container */
  /* display: inline-flex; */ /* inline flex container */

  display : flex | inline-flex; 
}
```

> **Syntax & Example**: `2.1-flex-display.html,  display: flex; /* block level flex container */`

```html
<!DOCTYPE html>

<html lang="en">

  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>2.1-flex-display</title>

    <style type="text/css">

      body {
        margin: 0;
        padding: 0;
        font-family: verdana;
      }

      .main-container {
        border: 4px solid #826a98;
        display: flex; /* block level flex container */
      }

      .item {
        color: #ffffff;
        font-size: 1rem;
        padding: 0.75rem;
        text-align: center;
      }

      .item-1 {
        background-color:#DDA0DD;
      }

      .item-2 {
        background-color:#BF94E4;
      }

      .item-3 {
        background-color:#734F96;
      }

      .item-4 {
        background-color:#FBAED2;
      }

      .item-5 {
        background-color:#EE82EE;
      }
      
      .item-6 {
        background-color:#ADE4CA;
      }

      .item-7 {
        background-color:#A6D5AE;
      }

      .item-8 {
        background-color:#8FBC8E;
      }

      .item-9 {
        background-color: #64A466;
      }
      
      .item-10 {
        background-color:#2E8B56;
      }

    </style>

  </head>

  <body>

    <div class="main-container">
      <div class="item item-1">item-1</div>
      <div class="item item-2">item-2</div>
      <div class="item item-3">item-3</div>
      <div class="item item-4">item-4</div>
      <div class="item item-5">item-5</div>
      <div class="item item-6">item-6</div>
      <div class="item item-7">item-7</div>
      <div class="item item-8">item-8</div>
      <div class="item item-9">item-9</div>
      <div class="item item-10">item-10</div>
    </div>
    
  </body>
  
</html>
```

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.1-flex-display-1-flex.png" alt="display: flex;" title="display: flex;" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - display: flex; </figcaption>
  </figure>
</p>

<hr/>

> **Syntax & Example**: `2.1-flex-display.html,  display: inline-flex; /* inline flex container */`

```css
.main-container {
  border: 4px solid #826a98;
  /* display: flex; */ /* block level flex container */
  display: inline-flex; /* inline flex container */ 
}
```

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.1-flex-display-2-inline-flex.png" alt="display: inline-flex;" title="display: inline-flex;" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - display: inline-flex; </figcaption>
  </figure>
</p>

2.2. Flex Direction
---------------------

- The flex-direction property decides/defines how flex items will stack inside flex container along the main axis, by default it's Main Axis runs from Left to Right
- Flex items can be laid out in two main directions, like rows horizontally or like columns vertically

`flex-direction` property sets the direction of the flex items along with the main axis:
- **`flex-direction: row`**;
  - Default direction is row-wise ie. left to right alignment
  - With row direction, the flex items are stacked in a row from left-to-right
- **`flex-direction: row-reverse`**;
  - Right to left alignment (item alignment will start from right to left - item 1 will start from right)
- **`flex-direction: column`**;
  - The column value stacks the flex items vertically (from top to bottom)
- **`flex-direction: column-reverse`**;
  - bottom to top (item alignment will start from bottom to top - item 1 will start from the bottom)
- syntax:
```css 
.container {
  display: inline-flex;
  
  flex-direction: row | row-reverse | column | column-reverse;
}
```

> **Syntax & Example**: `2.2-flex-direction.html, flex-direction: row; /* left to right */`

```html
<!DOCTYPE html>

<html lang="en">

  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>2.2-flex-direction</title>

    <style type="text/css">

      body {
        margin: 0;
        padding: 0;
        font-family: verdana;
      }

      .main-container {
        border: 4px solid #826a98;
        /* display: flex; */ /* block level flex container */
        display: inline-flex; /* inline flex container */
        
        /* flex-direction: row; */ /* left to right */
        /* flex-direction: row-reverse; */ /* right to left */
        /* flex-direction: column; */ /* top to bottom */
        flex-direction: column-reverse; /* bottom to top */
      }

      .item {
        color: #ffffff;
        font-size: 1rem;
        padding: 0.75rem;
        text-align: center;
      }

      .item-1 {
        background-color:#DDA0DD;
      }

      .item-2 {
        background-color:#BF94E4;
      }

      .item-3 {
        background-color:#734F96;
      }

      .item-4 {
        background-color:#FBAED2;
      }

      .item-5 {
        background-color:#EE82EE;
      }
      
      .item-6 {
        background-color:#ADE4CA;
      }

      .item-7 {
        background-color:#A6D5AE;
      }

      .item-8 {
        background-color:#8FBC8E;
      }

      .item-9 {
        background-color: #64A466;
      }
      
      .item-10 {
        background-color:#2E8B56;
      }

    </style>

  </head>

  <body>

    <div class="main-container">
      <div class="item item-1">item-1</div>
      <div class="item item-2">item-2</div>
      <div class="item item-3">item-3</div>
      <div class="item item-4">item-4</div>
      <div class="item item-5">item-5</div>
      <div class="item item-6">item-6</div>
      <div class="item item-7">item-7</div>
      <div class="item item-8">item-8</div>
      <div class="item item-9">item-9</div>
      <div class="item item-10">item-10</div>
    </div>
    
  </body>
  
</html>
```

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.2-flex-direction-1-row.png" alt="flex-direction: row;" title="flex-direction: row;" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - flex-direction: row; </figcaption>
  </figure>
</p>

<hr/>

<p>
  <figure>
  &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.2-flex-direction-2-row-reverse.png" alt="flex-direction: row-reverse;" title="flex-direction: row-reverse;" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - flex-direction: row-reverse; </figcaption>
  </figure>
</p>

<hr/>

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.2-flex-direction-3-column.png" alt="flex-direction: column;" title="flex-direction: column;" height="500" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - flex-direction: column; </figcaption>
  </figure>
</p>

<hr/>

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.2-flex-direction-4-column-reverse.png" alt="flex-direction: column-reverse;" title="flex-direction: column-reverse;" height="500" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - flex-direction: column-reverse; </figcaption>
  </figure>
</p>

2.3. Flex Wrap
---------------------

By default, all items in Flex Container try to fit themselves in a container in one row/column. If enough space not available, items simply overflow - with the help of `flex-wrap` property we can set the overflow direction 

- The `flex-wrap` property specifies whether the flex items should wrap or not
- The `flex-wrap` property simply determines how items are wrapped when the parent container runs out of space

`flex-wrap` property controls the wrapping of flex items within the container:
- **`flex-wrap: nowrap;`** (default is row nowrap)
- **`flex-wrap: wrap;`** (wraps overflow items to bottom/next row or right/next column)
- **`flex-wrap: wrap-reverse;`** (wraps overflow items to top row or left column)
- syntax:
```css
.container {
  display: inline-flex;
  
  flex-wrap: nowrap | wrap | wrap-reverse;
}
```

### 2.3.1. Row wise flex-wrap

> **Syntax & Example**: `2.3.1-flex-wrap-row.html flex-wrap: wrap; /* wraps overflow items to bottom/next row */`

```css
.main-container {
  border: 4px solid #826a98;
  display: flex; /* block level flex container */

  /* flex-wrap: nowrap; */ /* default is row nowrap */
  /* flex-wrap: wrap; */ /* wraps overflow items to bottom/next row */
  flex-wrap: wrap-reverse; /* wraps overflow items to top row */
}
```

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.3.1.1-flex-wrap-row.png" alt="flex-wrap: wrap;" title="flex-wrap: wrap" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - row flex-wrap: wrap; </figcaption>
  </figure>
</p>

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.3.1.2-flex-wrap-row-reverse.png" alt="flex-wrap: wrap-reverse;" title="flex-wrap: wrap-reverse;" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - row flex-wrap: wrap-reverse; </figcaption>
 </figure>
</p>

<hr/>

### 2.3.2. Columner/Column wise flex-wrap

> **Syntax & Example**: `2.3.2-flex-wrap-column.html flex-wrap: wrap; /* wraps overflow items to right/next column */`

```css
.main-container {
  border: 4px solid #826a98;
  display: flex; /* block level flex container */

  height: 300px;
  flex-direction: column;
  /* flex-wrap: nowrap; */ /* default is nowrap */
  /* flex-wrap: wrap; */ /* wraps overflow items to right/next column */
  flex-wrap: wrap-reverse; /* wraps overflow items to left column */
}
```

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.3.2.1-flex-wrap-column.png" alt="flex-wrap: wrap" title="flex-wrap: wrap" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - column flex-wrap: wrap; </figcaption>
  </figure>
</p>

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.3.2.2-flex-wrap-column-reverse.png" alt="flex-wrap: wrap-reverse" title="flex-wrap: wrap-reverse" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - column flex-wrap: wrap-reverse; </figcaption>
  </figure>
</p>

2.4. Flex Flow
---------------------

- `flex-flow` property is shorthand for `flex-direction` and `flex-wrap` properties
- By default `flex-flow` property is set to `row` and `nowrap` which is default value of properties like `flex-direction` and `flex-wrap`
- syntax:
```css
.container {
  /* flex-flow: <flex-direction> && <flex-wrap> */
  flex-flow: row wrap;
}
```

### 2.4.1. Row wise - flex-flow: row wrap

> **Syntax & Example**: `2.4.1-flex-flow-row.html`

```css
.main-container {
  border: 4px solid #826a98;
  display: flex; /* block level flex container */
  
  /* basic or normal way for row wrap */
  /* flex-direction: row; */
  /* flex-wrap: wrap; */

  /* latest way to write and use flex-flow, instead of flex-direction and flex-wrap */
  /* flex-flow: row wrap; */
  /* flex-flow: row wrap-reverse; */
  flex-flow: row-reverse wrap-reverse;
}
```

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.4.1.1-flex-flow-row-wrap.png" alt="flex-flow: row wrap;" title="flex-flow: row wrap;" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - flex-flow: row wrap; </figcaption>
  </figure>
</p>

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.4.1.2-flex-flow-row-reverse-wrap.png" alt="flex-flow: row-reverse wrap;" title="flex-flow: row-reverse wrap;" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - flex-flow: row-reverse wrap; </figcaption>
 </figure>
</p>

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.4.1.3-flex-flow-row-reverse-wrap-reverse.png" alt="flex-flow: row-reverse wrap-reverse;" title="flex-flow: row-reverse wrap-reverse;" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - flex-flow: row-reverse wrap-reverse; </figcaption>
 </figure>
</p>

<hr/>

### 2.4.2. Column wise - flex-flow: column wrap

> **Syntax & Example**: `2.4.2-flex-flow-column.html`

```css
.main-container {
  border: 4px solid #826a98;
  display: flex; /* block level flex container */
  
  /* basic or normal way for row wrap */
  /* flex-direction: row; */
  /* flex-wrap: wrap; */
  /* height: 300px; */

  /* latest way to write and use flex-flow, instead of flex-direction and flex-wrap */
  height: 300px;
  flex-flow: column wrap;
  /* flex-flow: column-reverse wrap; */
  /* flex-flow: column-reverse wrap-reverse; */
}
```

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.4.2.1-flex-flow-column-wrap.png" alt="flex-flow: column wrap;" title="flex-flow: column wrap;" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - flex-flow: column wrap; </figcaption>
  </figure>
</p>

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.4.2.2-flex-flow-column-reverse-wrap.png" alt="flex-flow: column-reverse wrap;" title="flex-flow: column-reverse wrap;" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - flex-flow: column-reverse wrap; </figcaption>
 </figure>
</p>

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.4.2.3-flex-flow-column-reverse-wrap-reverse.png" alt="flex-flow: column-reverse wrap-reverse;" title="flex-flow: column-reverse wrap-reverse;" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - flex-flow: column-reverse wrap-reverse; </figcaption>
 </figure>
</p>

2.5. Justify Content
---------------------

- `justify-content` defines and set the alignment of flex items along with the main axis
- It helps distribute extra free space leftover when either all the flex items on a line
- The default value of `justify-content` is `flex-start` which simply means start all flex items from left side exactly the place where the container starts (`justify-content: flex-start;`)
- syntax:
```css
.container {
  justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly | start | end | left | right
}
```

`justify-content` property is used to align the flex items within the container along with the main axis:
- **`justify-content: flex-start;`**
  - Default alignment for items, start from/packed toward the left side of the container
  - The `flex-start` value aligns the flex items at the beginning of the container (this is the default)
- **`justify-content: flex-end;`**
  - Align item to right or end of the container main axis
- **`justify-content: center`**
  - Align item at the center of the main container 
  - `center` value aligns the flex items at the center of the container
- **`justify-content: space-between`**
  - Equally, distribute the items [(apart from first-start and last-end item) in between items will be distributed with equal gap/space ]
- **`justify-content: space-around`**
  - `space-around` property displays the flex items with space before, between, and after the lines
  - [( first-start and last-end items have 50% space/gap) in between items will be distributed with 100% gap/space ]
  - [space to the edges will be 50% ] and spacing between any two items are 100%
- **`justify-content: space-evenly`**
  - All flex item is distributed with even/equal space-gap
  - All flex items are distributed evenly/equally so that the spacing between any two items (and the space to the edges) is also equal

### 2.5.1. Row wise justify-content

> **Syntax & Example**: `2.5.1-flex-justify-content-row.html`

```css
.main-container {
  border: 4px solid #826a98;
  display: flex; /* block level flex container */
  
  /*  justify-content: flex-start; */
  /* justify-content: flex-end; */
  /* justify-content: center; */
  /* justify-content: space-between; */
  /* justify-content: space-around; */
  justify-content: space-evenly;
}
```

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.5.1.1-flex-justify-content-row-flex-start.png" alt="justify-content: flex-start;" title="justify-content: flex-start;" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - justify-content: flex-start; </figcaption>
  </figure>
</p>

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.5.1.2-flex-justify-content-row-flex-end.png" alt="justify-content: flex-end;" title="justify-content: flex-end;" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - justify-content: flex-end; </figcaption>
  </figure>
</p>

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.5.1.3-flex-justify-content-row-center.png" alt="justify-content: center;" title="justify-content: center;" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - justify-content: center; </figcaption>
  </figure>
</p>

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.5.1.4-flex-justify-content-row-space-between.png" alt="justify-content: space-between;" title="justify-content: space-between;" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - justify-content: space-between; </figcaption>
  </figure>
</p>

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.5.1.5-flex-justify-content-row-space-around.png" alt="justify-content: space-around;" title="justify-content: space-around;" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - justify-content: space-around; </figcaption>
  </figure>
</p>

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.5.1.6-flex-justify-content-row-space-evenly.png" alt="justify-content: space-evenly;" title="justify-content: space-evenly;" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - justify-content: space-evenly; </figcaption>
  </figure>
</p>

<hr/>

### 2.5.2. Columner/Column wise justify-content

> **Syntax & Example**: `2.5.2-flex-justify-content-column.html`

```css
.main-container {
  border: 4px solid #826a98;
  display: flex; /* block level flex container */
  
  flex-direction: column;
  height: 600px;
  /* justify-content: flex-start; */
  /* justify-content: flex-end; */
  /* justify-content: center; */
  /* justify-content: space-between; */
  /* justify-content: space-around; */
  justify-content: space-evenly;
}
```

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.5.2.1-flex-justify-content-column-flex-start.png" alt="justify-content: flex-start;" title="justify-content: flex-start;" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - justify-content: flex-start; </figcaption>
  </figure>
</p>

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.5.2.2-flex-justify-content-column-flex-end.png" alt="justify-content: flex-end;" title="justify-content: flex-end;" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - justify-content: flex-end; </figcaption>
  </figure>
</p>

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.5.2.3-flex-justify-content-column-center.png" alt="justify-content: center;" title="justify-content: center;" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - justify-content: center; </figcaption>
  </figure>
</p>

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.5.2.4-flex-justify-content-column-space-between.png" alt="justify-content: space-between;" title="justify-content: space-between;" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - justify-content: space-between; </figcaption>
  </figure>
</p>

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.5.2.5-flex-justify-content-column-space-around.png" alt="justify-content: space-around;" title="justify-content: space-around;" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - justify-content: space-around; </figcaption>
  </figure>
</p>

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.5.2.6-flex-justify-content-column-space-evenly.png" alt="justify-content: space-evenly;" title="justify-content: space-evenly;" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - justify-content: space-evenly; </figcaption>
  </figure>
</p>

2.6. Align Items
---------------------

- `align-items` property defines default behavior of flex items, it simply means how flex items align along the cross axis (vertically) of the container
- `align-items` is similar to justify-content but works in a perpendicular direction to the main-axis
- syntax:
```css
.container {
  align-items: stretch | flex-start | flex-end | center | baseline 
}
```

The `align-items` property will align the items on the cross axis:
- **`align-item: stretch;`**
  - Default alignment for flex-items, covers/occupy 100% height of container
- **`align-item: flex-start;`**
  - All flex items squeezed/stacked or align at start ie. from the top of the container (items line up at the start of the flex container)
- **`align-item: flex-end;`**
  - All flex items start/stacked from bottom or aligned/pushed at the bottom
- **`align-item: center;`**
  - Align item vertically center/middle of the container (items are stacked to the center/middle of the container)
- **`align-item: baseline;`**
  - The baseline is the line upon which most of the letter set (Flex items are aligned in a way that their baselines are aligned)

### 2.6.1. Row wise align-item

> **Syntax & Example**: `2.6.1-flex-align-item-row.html`

```html
<!DOCTYPE html>

<html lang="en">

  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>2.6.1-flex-align-item-row</title>

    <style type="text/css">

      body {
        margin: 0;
        padding: 0;
        font-family: verdana;
      }

      .main-container {
        border: 4px solid #826a98;
        
        display: flex; /* block level flex container */
        height: 600px;

        align-items: stretch;  /* default value for algn-iitems is stretch */
        /* align-items: flex-start; */
        /* align-items: flex-end; */
        /* align-items: center; */
        /* align-items: baseline; */
      }

      .item {
        color: #ffffff;
        font-size: 1rem;
        padding: 0.75rem;
        text-align: center;
      }

      .item-1 {
        background-color:#DDA0DD;
        padding-bottom: 2rem;
      }

      .item-2 {
        background-color:#BF94E4;
        padding-bottom: 3rem;
      }

      .item-3 {
        background-color:#734F96;
        font-size: 3rem;
      }

      .item-4 {
        background-color:#FBAED2;
      }

      .item-5 {
        background-color:#EE82EE;
      }
      
      .item-6 {
        background-color:#ADE4CA;
      }

      .item-7 {
        background-color:#A6D5AE;
      }

      .item-8 {
        background-color:#8FBC8E;
      }

      .item-9 {
        background-color: #64A466;
      }
      
      .item-10 {
        background-color:#2E8B56;
      }

    </style>

  </head>

  <body>

    <div class="main-container">
      <div class="item item-1">item-1</div>
      <div class="item item-2">item-2</div>
      <div class="item item-3">item-3</div>
      <div class="item item-4">item-4</div>
      <div class="item item-5">item-5</div>
      <div class="item item-6">item-6</div>
      <div class="item item-7">item-7</div>
      <div class="item item-8">item-8</div>
      <div class="item item-9">item-9</div>
      <div class="item item-10">item-10</div>
    </div>
    
  </body>
  
</html>
```

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.6.1.1-flex-align-item-row-stretch.png" alt="align-items: stretch;" title="align-items: stretch;" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - align-items: stretch; </figcaption>
  </figure>
</p>

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.6.1.2-flex-align-item-row-flex-start.png" alt="align-items: flex-start;" title="align-items: flex-start;" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - align-items: flex-start; </figcaption>
  </figure>
</p>

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.6.1.3-flex-align-item-row-flex-end.png" alt="align-items: flex-end;" title="align-items: flex-end;" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - align-items: flex-end; </figcaption>
  </figure>
</p>

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.6.1.4-flex-align-item-row-center.png" alt="align-items: center;" title="align-items: center;" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - align-items: center; </figcaption>
  </figure>
</p>

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.6.1.5-flex-align-item-row-baseline.png" alt="align-items: baseline;" title="align-items: baseline;" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - align-items: baseline; </figcaption>
  </figure>
</p>

<hr/>

### 2.6.2. Columner/Column wise align-item

> **Syntax & Example**: `2.6.2-flex-align-item-column.html`

```html
<!DOCTYPE html>

<html lang="en">

  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>2.6.2-flex-align-item-column</title>

    <style type="text/css">

      body {
        margin: 0;
        padding: 0;
        font-family: verdana;
      }

      .main-container {
        border: 4px solid #826a98;
        
        display: flex; /* block level flex container */
        flex-direction: column;
        height: 600px;
        
        /* align-items: stretch; */  /* default value for algn-iitems is stretch */
        /* align-items: flex-start; */
        /* align-items: flex-end; */
        /* align-items: center; */
        align-items: baseline;
      }

      .item {
        color: #ffffff;
        font-size: 1rem;
        padding: 0.75rem;
        text-align: center;
      }

      .item-1 {
        background-color:#DDA0DD;
        padding-bottom: 2rem;
        font-family:cursive;
      }

      .item-2 {
        background-color:#BF94E4;
        padding-bottom: 3rem;
        padding-right: 5rem;
      }

      .item-3 {
        background-color:#734F96;
        font-size: 3rem;
      }

      .item-4 {
        background-color:#FBAED2;
        font-size: 8px;
      }

      .item-5 {
        background-color:#EE82EE;
      }
      
      .item-6 {
        background-color:#ADE4CA;
      }

      .item-7 {
        background-color:#A6D5AE;
      }

      .item-8 {
        background-color:#8FBC8E;
      }

      .item-9 {
        background-color: #64A466;
      }
      
      .item-10 {
        background-color:#2E8B56;
      }

    </style>

  </head>

  <body>

    <div class="main-container">
      <div class="item item-1">item-1</div>
      <div class="item item-2">item-2</div>
      <div class="item item-3">item-3</div>
      <div class="item item-4">item-4</div>
      <div class="item item-5">item-5</div>
      <div class="item item-6">item-6</div>
      <div class="item item-7">item-7</div>
      <div class="item item-8">item-8</div>
      <div class="item item-9">item-9</div>
      <div class="item item-10">item-10</div>
    </div>
    
  </body>
  
</html>
```

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.6.2.1-flex-align-item-column-stretch.png" alt="align-items: stretch;" title="align-items: stretch;" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - align-items: stretch; </figcaption>
  </figure>
</p>

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.6.2.2-flex-align-item-column-flex-start.png" alt="align-items: flex-start;" title="align-items: flex-start;" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - align-items: flex-start; </figcaption>
  </figure>
</p>

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.6.2.3-flex-align-item-column-flex-end.png" alt="align-items: flex-end;" title="align-items: flex-end;" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - align-items: flex-end; </figcaption>
  </figure>
</p>

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.6.2.4-flex-align-item-column-center.png" alt="align-items: center;" title="align-items: center;" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - align-items: center; </figcaption>
  </figure>
</p>

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="_images-css-flexbox/2.6.2.5-flex-align-item-column-baseline.png" alt="align-items: baseline;" title="align-items: baseline;" width="1000" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - align-items: baseline; </figcaption>
  </figure>
</p>
