
## **1. What is HTML?**

* **HTML (HyperText Markup Language)** is the standard language used to create web pages.
* It uses a system of "tags" to define elements on a page (such as headings, paragraphs, links, etc.).

---

## **2. Basic HTML Structure**

Every HTML page begins with a basic structure that includes these key elements:

```html
<!DOCTYPE html>  <!-- Specifies the document type and version (HTML5) -->
<html>           <!-- Root element of the HTML page -->
<head>           <!-- Contains meta-information about the document (title, links, etc.) -->
    <meta charset="UTF-8">  <!-- Specifies character encoding (UTF-8 for global text support) -->
    <title>Page Title</title>  <!-- Title of the page, visible in browser tab -->
</head>
<body>           <!-- Main content of the HTML page -->
    <!-- Content goes here -->
</body>
</html>
```

---

## **3. Basic Tags and Elements**

### **a. Text Formatting**

* **Headings**: HTML offers 6 levels of headings (`<h1>` to `<h6>`).

  ```html
  <h1>This is the largest heading</h1>
  <h2>This is a smaller heading</h2>
  ```

* **Paragraphs**: Use `<p>` for paragraphs.

  ```html
  <p>This is a paragraph of text.</p>
  ```

* **Bold and Italic**:

  * Bold: `<strong>` or `<b>`
  * Italic: `<em>` or `<i>`

  ```html
  <strong>This text is bold</strong>
  <em>This text is italic</em>
  ```

* **Line Break**: `<br>` to add line breaks.

  ```html
  Line one<br>Line two
  ```

* **Lists**:

  * Unordered List (`<ul>`): List items with bullet points.

    ```html
    <ul>
        <li>Item 1</li>
        <li>Item 2</li>
    </ul>
    ```
  * Ordered List (`<ol>`): List items with numbers.

    ```html
    <ol>
        <li>First item</li>
        <li>Second item</li>
    </ol>
    ```

---

### **b. Links and Images**

* **Links**: Use `<a>` to create hyperlinks.

  ```html
  <a href="https://www.example.com">Go to Example</a>
  ```

* **Images**: Use `<img>` to add images (with `src` for the source and `alt` for alternative text).

  ```html
  <img src="image.jpg" alt="Description of the image">
  ```

---

### **c. Forms**

* **Form Elements**: Use `<form>` for collecting user input. Common elements include text fields (`<input>`), text areas (`<textarea>`), and buttons (`<button>`).

  ```html
  <form>
      <label for="name">Name:</label>
      <input type="text" id="name" name="name">
      <button type="submit">Submit</button>
  </form>
  ```

---

## **4. HTML Attributes**

Attributes provide additional information about an HTML element. They're always written inside the opening tag.

* **`id`**: Unique identifier for an element.

  ```html
  <div id="header">This is a div with an ID.</div>
  ```

* **`class`**: Used for applying styles to multiple elements.

  ```html
  <div class="box">This is a div with a class.</div>
  ```

* **`style`**: Inline CSS (not recommended for large-scale styling).

  ```html
  <p style="color: blue;">This text is blue.</p>
  ```

* **`href`**: Used in `<a>` tags to specify the link's destination.

  ```html
  <a href="https://www.example.com">Visit Example</a>
  ```

---

## **5. Media Elements**

* **Audio**:

  ```html
  <audio controls>
      <source src="audiofile.mp3" type="audio/mp3">
  </audio>
  ```

* **Video**:

  ```html
  <video width="320" height="240" controls>
      <source src="video.mp4" type="video/mp4">
  </video>
  ```

---

## **6. HTML Comments**

* Comments are useful for notes within your code, and they don't show up on the page.

  ```html
  <!-- This is a comment -->
  ```

---

## **7. Div and Span**

* **`<div>`**: Used for grouping elements (block-level element).

  ```html
  <div>
      <h2>This is a heading inside a div</h2>
      <p>This is a paragraph inside a div.</p>
  </div>
  ```

* **`<span>`**: Used for grouping inline elements (inline-level element).

  ```html
  <p>This is a <span style="color: red;">red</span> word.</p>
  ```

---

## **8. Tables**

Tables are defined using the following tags:

```html
<table>
    <tr> <!-- Table row -->
        <th>Header 1</th> <!-- Table header -->
        <th>Header 2</th>
    </tr>
    <tr>
        <td>Data 1</td> <!-- Table data -->
        <td>Data 2</td>
    </tr>
</table>
```

---

### **9. Semantic HTML Elements**

Semantic elements describe the meaning of the content they contain.

* `<header>`: Defines a header for a document or section.
* `<footer>`: Defines a footer for a document or section.
* `<article>`: Defines an independent section of content.
* `<section>`: Defines a section in the document.

Example:

```html
<header>
    <h1>Website Header</h1>
</header>
<article>
    <h2>Article Title</h2>
    <p>Content of the article...</p>
</article>
<footer>
    <p>Website Footer</p>
</footer>
```

---

## **10. Conclusion**

HTML is a markup language that structures content on the web. You can create pages with text, images, links, and more using various HTML tags. Once you're familiar with the basic tags, you can start integrating CSS and JavaScript to add styling and interactivity.

