# CSS Selectors

### 1. **Basic Selectors**

#### a. **Element Selector**
The element selector targets all elements of a specific type.
```css
p {
  color: blue;
}
```
This will set the text color to blue for all `<p>` elements in the document.

#### b. **ID Selector**
The ID selector targets a specific element with a unique ID. Use the `#` symbol followed by the ID name.
```css
#header {
  background-color: yellow;
}
```
This applies a yellow background color to the element with `id="header"`. Remember that IDs should be unique in a document.

#### c. **Class Selector**
The class selector targets elements that have a specific class attribute. Use the `.` symbol followed by the class name.
```css
.button {
  font-size: 16px;
}
```
This will style all elements with `class="button"` to have a font size of 16px. Multiple elements can have the same class.

### 2. **Combinator Selectors**

#### a. **Descendant Selector**
The descendant selector is used to select elements that are inside a specific element.
```css
div p {
  color: red;
}
```
This targets all `<p>` elements inside `<div>` elements and changes their color to red.

#### b. **Child Selector**
The child selector (`>`) selects elements that are direct children of a specified element.
```css
ul > li {
  list-style: none;
}
```
This targets `<li>` elements that are direct children of a `<ul>` and removes their bullet points.

#### c. **Adjacent Sibling Selector**
The adjacent sibling selector (`+`) selects an element that is immediately following a specified element.
```css
h2 + p {
  margin-top: 0;
}
```
This selects the `<p>` element that directly follows an `<h2>` and sets its top margin to 0.

#### d. **General Sibling Selector**
The general sibling selector (`~`) selects all elements that are siblings of a specified element.
```css
h2 ~ p {
  color: green;
}
```
This will style all `<p>` elements that are siblings of an `<h2>` element.

### 3. **Attribute Selectors**

Attribute selectors target elements based on their attributes.

#### a. **[attribute] Selector**
Selects elements that have a specific attribute.
```css
input[type="text"] {
  border: 1px solid black;
}
```
This targets `<input>` elements where `type="text"` and adds a border.

#### b. **[attribute^="value"] Selector**
Selects elements where the attribute starts with a specific value.
```css
a[href^="https"] {
  color: blue;
}
```
This targets `<a>` elements whose `href` attribute starts with "https".

#### c. **[attribute$="value"] Selector**
Selects elements where the attribute ends with a specific value.
```css
img[src$=".png"] {
  width: 200px;
}
```
This targets `<img>` elements where the `src` attribute ends with ".png".

### 4. **Pseudo-Class Selectors**

Pseudo-classes are used to define a special state of an element.

#### a. **:hover**
Targets an element when the mouse hovers over it.
```css
a:hover {
  color: red;
}
```
This changes the color of a link when it is hovered over.

#### b. **:first-child**
Selects an element that is the first child of its parent.
```css
p:first-child {
  font-weight: bold;
}
```
This targets the first `<p>` element inside its parent and makes it bold.

#### c. **:nth-child(n)**
Selects elements based on their position in a parent.
```css
li:nth-child(odd) {
  background-color: lightgray;
}
```
This targets odd-numbered `<li>` elements and gives them a light gray background.

### 5. **Pseudo-Element Selectors**

Pseudo-elements are used to style parts of an element.

#### a. **::before**
Inserts content before an element.
```css
p::before {
  content: "Note: ";
  font-weight: bold;
}
```
This adds "Note: " before every `<p>` element.

#### b. **::after**
Inserts content after an element.
```css
button::after {
  content: " ✓";
}
```
This adds a checkmark after every `<button>` element.

### Summary
CSS selectors allow you to target HTML elements in a variety of ways. By using a combination of element, class, ID, combinator, attribute, pseudo-class, and pseudo-element selectors, you can create precise styles for your web pages.

Here’s a quick reference:

- **Element**: `div`, `p`, etc.
- **ID**: `#header`
- **Class**: `.button`
- **Combinators**: `div p` (descendant), `ul > li` (child)
- **Attribute**: `[type="text"]`, `[href^="https"]`
- **Pseudo-class**: `a:hover`, `p:first-child`
- **Pseudo-element**: `p::before`, `button::after`

Understanding and using these selectors effectively will make your CSS much more powerful and flexible.

#2404/webdesign