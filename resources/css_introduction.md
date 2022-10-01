# CSS = Cascading Style Sheets

It is used to style and lay out web pages - for example, to alter the font, color, size, and spacing of your content, split it into multiple columns, or add animations and other decorative features.

### CSS rules

It is structured like this 
```
selector {
    property1: value1;
    property2: value2;
}
```

A selector is used to target the HTML element on the web page. The elements that are inside the parentheses describe how the properties are modified.

Example:
```
p {
    color: blue
}
```

CSS can be included in 3 ways:
* External file - needs to be referenced in the HTML's head using the link tag: ```<link rel="stylesheet" href="styles.css" />```
* Embedded/Internal - open a style tag inside HTML's head: ```<style>...</style>```
* Inline - add a style attribute directly to a HTML element: ```<h1 style="color:blue;text-align:center;">Inline styled heading!</h1> ``` (Not really recommended)

Selectors can be:
* HTML elements: ```p { ... } ```,
* Class: ``` .class-selector { ... } ``` it is also need to reference this class to the elements that use it: ``` <p className="class-selector">...</p>```,
* Ids - similar to class - ``` #id-selector { ... } ```, ``` <p id="id-selector">...</p>``` (Not really recommended).

Selectors can also be combined (grouping selectors):
```
h1, p,
.class-selector {
  color: blue;
}
```

There are also pseudo-classes and pseudo-elements like:
```
a:hover {
}

p::first-line {
}
```

And other combinations: 
```
article > p {
}

input[type="button"] {
}
```

### CSS Units
There are two types of length units: **absolute and relative**. Some properties can also have negative length.

The absolute length units are fixed.

Relative length units specify a length relative to another length property. Relative length units scale better between different rendering medium.

Most popular units are:
* px - pixels (absolute but with a catch because it takes into account the viewing device),
* em - relative to the font-size of the element (2em means 2 times the size of the current font),
* rem - relative to font-size of the root element,
* vw, vh - relative to 1% of the width or height of the viewport (viewport = the browser window size. If the viewport is 50cm wide, 1vw = 0.5cm.),
* % - Relative to the parent element.

### Common properties
```
Font:
p.a {
  font: 15px Arial, sans-serif;
}

Margin:
p {
  margin-top: 100px;
  margin-bottom: 100px;
  margin-right: 150px;
  margin-left: 80px;
}

Border:
p.solid { border-style: solid; }

Padding:
div {
  padding-top: 50px;
  padding-right: 30px;
  padding-bottom: 50px;
  padding-left: 80px;
}

Dimensions:
div {
  height: 100px;
  width: 500px;
}

Layout control:
div {
    display: block | flex | grid | table;
}

img {
  float: right;
}

Position control:
div {
    position: static | relative | absolute | fixed | sticky;
}
```