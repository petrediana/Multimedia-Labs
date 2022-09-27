# HTML = Hyper Text Markup Language

HyperText - means that document contains links
Markup Language - a way that computers control how the text is processed and presented.

HTML uses two things to achieve this: **tags and attributes**.

### Tags

They mark the start of an element and are enclosed in angle brackets. Usually, tags need to be also closed.

```
<h1>Hello!</h1>
```

When using multiple tags, the tags must be closed in the order in which they were opened.

```
<div>
    <h1>Hello!</h1>
</div>
```

### Attributes

They contain additional information, such as an image source. Attributes are placed inside the tag.

```
<img src="some_image.jpg" alt="Some image" width="420" height="420">
```

### HTML Page
```
<!DOCTYPE html>
<html>
<head>
<title>Title of the document</title>
</head>

<body>
Content of the document
</body>
</html>
```

### Elements

Headings: ```<h1>, <h2>, <h3>, <h4>, <h5>, <h6>```

Anchor Tag: ```<a href="www.google.com">Click me!</a> ```

Image Tag: ``` <img src="folder/img.jpg" alt="Image" height="10" width="15"> ```

Form element & Tag:
```
<form>
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe">
</form>
```

Canvas Tag:
```
<canvas></canvas>
```

SVG (Scalable Vector Graphics) Tag:
```
<svg width="100" height="100">
  <circle cx="50" cy="50" r="40" stroke="green" stroke-width="4" fill="yellow" />
</svg>
```

Video Tag:
```
<video width="320" height="240" controls>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
  Video tag not supported :(
</video>
```

Lists - Ordered: 
```
<ol>
    <li>First item<li>
    <li>Second item<li>
    <li>Third item<li>
</ol>
```

Lists - Unordered (Bullet point list):
```
<ul>
    <li>This is </li>
    <li>An Unordered </li>
    <li>List </li>
</ul>
```

Lists - Definition List:
```
<dl>
    <dt>Item</dt>
    <dd>The definition goes here</dd>
</dl>
```

Table - simple:
```
<table>
    <tr>
    <th>Column header 1</th>
    <th>Column header 2</th>
    </tr>
    <tr>
        <td>Row 1 - Column 1</td>
        <td>Row 1 - Column 2 </td>
    </tr>
    <tr>
        <td>Row 2 - Column 1</td>
        <td>Row 2 - Column 2</td>
    </tr>
</table>
```

Table - more complex:
```
<table>
  <caption>Some cool information</caption>
  <thead>
    <tr>
      <th>Column head</th>
      <th>Column head</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Hello</td>
      <td>World</td>
    </tr> 
  </tbody> 
  <tfoot>
    <tr>
    <td>Other cool info!</td>
    </tr>
  </tfoot>
</table>
```




