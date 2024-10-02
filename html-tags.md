# HTML Tags

## Anatomy of an HTML Tag

HTML (Hypertext Markup Language) is the standard language for creating webpages. It consists of elements that structure the content of a page. Each element is represented by HTML tags, which define how the content should be displayed. Let’s break down the components of an HTML tag.

#### 1. Opening and Closing Tags

Most HTML elements consist of an **opening tag** and a **closing tag**:

- **Opening Tag**: This indicates the beginning of an element and consists of the element name enclosed in angle brackets (`< >`).
  
  ```html
  <p>
  ```

  In this example, `<p>` represents an opening tag for a paragraph.

- **Closing Tag**: This indicates the end of an element and is similar to the opening tag, but with a forward slash (`/`) before the element name.

  ```html
  </p>
  ```

  Here, `</p>` represents a closing tag for a paragraph.

- **Content Between Tags**: The content goes between the opening and closing tags.

  ```html
  <p>This is a paragraph.</p>
  ```

#### 2. Attributes

Attributes provide additional information about an element and are included within the opening tag. Attributes consist of a **name** and a **value**, where the value is enclosed in quotation marks.

Syntax: `<element attribute="value">`

Example:
```html
<a href="https://example.com">Visit Example</a>
```

- `<a>` is an anchor tag used for hyperlinks.
- `href` is an attribute that specifies the URL to which the link points.
- `"https://example.com"` is the value of the `href` attribute.

Multiple attributes can be added to an element, separated by spaces:

```html
<img src="image.jpg" alt="A description of the image" width="300">
```

#### 3. Nesting Elements

Elements can be **nested** inside one another to create more complex structures. Nested elements must be properly closed in the correct order.

Example:

```html
<div>
  <h1>Welcome to My Website</h1>
  <p>This is a paragraph inside a div.</p>
</div>
```

In the example above:

- `<div>` is a container element that holds other elements (`<h1>` and `<p>`).
- The `<h1>` and `<p>` elements are **nested** inside the `<div>`.

> **Note**: Proper nesting means closing the inner tags before closing the outer tags. For example:

Correct nesting:
```html
<b><i>Bold and italic text</i></b>
```

Incorrect nesting:
```html
<b><i>Bold and italic text</b></i>
```

#### 4. Self-Closing Tags

Some HTML elements do not have any content, and thus do not need a closing tag. These are known as **self-closing tags**. In modern HTML (HTML5), these tags can be written without a forward slash.

Example:

```html
<img src="image.jpg" alt="A description of the image">
<br>
```

The `<img>` and `<br>` tags are examples of self-closing tags.

### Summary

- **Opening Tag**: Marks the start of an element (`<tag>`).
- **Closing Tag**: Marks the end of an element (`</tag>`).
- **Attributes**: Provide additional information about an element (`<tag attribute="value">`).
- **Nesting**: Elements can be nested inside each other but must be properly closed in the correct order.
- **Self-Closing Tags**: Tags that don’t need a closing tag (e.g., `<img>`).

Understanding the anatomy of an HTML tag will help you build structured and well-formed HTML documents.

## Most used HTML Tags

### 1. `<p>`: Paragraph
The `<p>` tag is used to define paragraphs in HTML. It's used to add blocks of text.

```html
<p>This is a paragraph of text.</p>
```

### 2. Headline Tags: `<h1>` to `<h6>`
Headline tags are used to define headings of different levels, from `<h1>` (most important) to `<h6>` (least important). 

```html
<h1>Main Heading (most important)</h1>
<h2>Subheading</h2>
<h3>Sub-subheading</h3>
<h4>...</h4>
<h5>...</h5>
<h6>Least Important Heading</h6>
```

- Use `<h1>` for the main title of the page.
- Use `<h2>` to `<h6>` for subheadings as needed.

### 3. `<ul>`: Unordered List
The `<ul>` tag is used to create an unordered list, typically styled as bullet points.

```html
<ul>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
</ul>
```

### 4. `<ol>`: Ordered List
The `<ol>` tag is used to create an ordered list, typically numbered.

```html
<ol>
    <li>Step 1</li>
    <li>Step 2</li>
    <li>Step 3</li>
</ol>
```

### 5. `<li>`: List Item
The `<li>` tag is used to define an item in either an ordered (`<ol>`) or unordered (`<ul>`) list. Each list item is enclosed in `<li>` tags.

### 6. `<img>`: Image
The `<img>` tag is used to embed an image in an HTML page. It is a self-closing tag and requires at least two attributes:
- `src`: The URL/path to the image.
- `alt`: Alternative text describing the image for accessibility.

```html
<img src="example.jpg" alt="Description of the image">
```

### 7. `<a>`: Anchor
The `<a>` tag is used to create hyperlinks. It requires an `href` attribute to specify the link's destination.

```html
<a href="https://www.example.com">Visit Example Website</a>
```

You can also use `<a>` to link to other parts of your page or to an email address.

### 8. `<div>`: Division
The `<div>` tag is used as a container for other HTML elements. It helps group and organize content and is commonly used for styling and layout purposes.

```html
<div>
    <h2>Section Title</h2>
    <p>This is some content inside a div.</p>
</div>
```

These tags form the foundation for structuring and organizing content on your web page.

You can find a comprehensive list of all HTML5 tags and their descriptions on the following resource:

[MDN Web Docs: HTML elements reference](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)

MDN Web Docs is an excellent reference maintained by Mozilla, providing detailed information about all HTML5 tags, their attributes, and usage examples.

### Summary

* **`<p>`**: Adds a paragraph of text.
* **Headlines (`<h1>` to `<h6>`)**: Defines headings from most important to least important.
* **`<ul>` and `<ol>`**: Define unordered (bulleted) and ordered (numbered) lists.
* **`<li>`**: Defines each item within a list.
* **`<img>`**: Embeds an image.
* **`<a>`**: Creates hyperlinks to other pages or locations.
* **`<div>`**: Groups content for styling and layout purposes.

