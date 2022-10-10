# Javascript

 Lightweight, cross-platform, and interpreted compiled programming language.
 
  JS can be used for Client-side developments as well as Server-side developments. JavaScript contains a standard library of objects, like Array, Date, and Math, and a core set of language elements like operators, control structures, and statements.

### Data types
- Primitives (immutable datum represented directly at the lowest level of the language):
    - Boolean type
    - Null type
    - Undefined type
    - Number type
    - BigInt type
    - String type
    - Symbol type
- Objects (collections of properties)

### Declaring variables
Keywords used: var, let, const.

### DOM manipulation

The browser pulls in HTML documents, parses them, and creates object models of the pages in its memory. This model is the Document Object Model (DOM). Each element in the HTML document is represented by a DOM node. These nodes can be accessed and changed using JavaScript.

When the model is updated, those changes are reflected on screen.

Methods that can be used to select an element or elements:

- ```document.querySelector("#id") ``` - returns the first Element within the document that matches the specified selector, or group of selectors. If no matches are found, null is returned,
- ```document.querySelectorAll('p')``` - returns a static (not live) NodeList representing a list of the document's elements that match the specified group of selectors.
- ```document.getElementById('id') ``` -  returns an Element object representing the element whose id property matches the specified string. Since element IDs are required to be unique if specified, they're a useful way to get access to a specific element quickly,
 - ```document.getElementsByClassName('class-name')``` -  returns an array-like object of all child elements which have all of the given class name(s). When called on the document object, the complete document is searched, including the root node. You may also call getElementsByClassName() on any element; it will return only elements which are descendants of the specified root element with the given class name(s),
 - ```document.getElementsByTagName('h1')``` - returns a live HTMLCollection of elements with the given tag name. All descendants of the specified element are searched, but not the element itself. The returned list is live, which means it updates itself with the DOM tree automatically.


Traversing the DOM:
- parentNode - locates the parent element of an initial selection,
- previousSibling - finds the previous sibling of a selected element,
- nextSibling - finds the next sibling of a selected element,
- firstChild - finds the first child of a selected element.

Accessing and Updating Content:
- innerHTML	- get or set the HTML content of an element,
- textContent - get or set the text content of an element.


### Events
Actions taken by a user that can trigger updates in the DOM.

Event Handlers:
We can set up event handlers in our scripts that will listen, or wait, for an event to occur and then trigger a function.

The syntax for setting up an event handler looks like this: ``` element.addEventListener('nameOfEvent', functionToRun); ```

Types of Events:
- 'click' - When a button (usually a mouse button) is pressed and released on a single element,
- 'keydown'	- When the user first presses a key on the keyboard,
- 'keyup' - When the user releases a key on the keyboard,
- 'focus' - When an element has received focus,
- 'blur' - When an element loses focus,
- 'submit' - When the user submits a form,
- 'load' - When the page has finished loading,
- 'resize' - When the browser window has been resized,
- 'scroll' - When the user scrolls up or down on the page,