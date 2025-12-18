
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

# CSS

## **1. What is CSS?**

* **CSS** is a stylesheet language used to describe the look and feel of a web page. It controls layout, colors, fonts, spacing, and more.
* CSS allows you to separate the structure (HTML) from the style (CSS), which makes maintaining and styling pages easier.

---

## **2. Basic CSS Syntax**

CSS uses **selectors** to target HTML elements and **properties** to apply styles to those elements.

```css
selector {
    property: value;
}
```

### Example:

```css
h1 {
    color: blue;
    font-size: 24px;
}
```

This would change all `<h1>` elements to blue and set their font size to 24px.

---

## **3. How to Include CSS in a Web Page**

There are three main ways to include CSS in an HTML document:

### **a. Inline CSS**

* Directly within an HTML element using the `style` attribute.

```html
<p style="color: red; font-size: 16px;">This is red text.</p>
```

### **b. Internal CSS**

* Inside a `<style>` tag within the `<head>` section of the HTML document.

```html
<head>
    <style>
        p {
            color: green;
        }
    </style>
</head>
```

### **c. External CSS**

* In a separate `.css` file linked to the HTML file using the `<link>` tag in the `<head>` section.

```html
<head>
    <link rel="stylesheet" href="styles.css">
</head>
```

Then, the CSS file (`styles.css`) would contain the styles:

```css
p {
    color: green;
}
```

---

## **4. CSS Selectors**

Selectors define which HTML elements the style rules apply to. Here are the most common ones:

### **a. Element Selector**

* Targets all instances of a specific element (e.g., all `<p>` tags).

```css
p {
    font-size: 18px;
}
```

### **b. Class Selector**

* Targets all elements with a specific class. A class is prefixed with a `.`.

```css
.box {
    border: 1px solid black;
}
```

HTML:

```html
<div class="box">Content inside box</div>
```

### **c. ID Selector**

* Targets a unique element with a specific `id`. An ID is prefixed with a `#`.

```css
#header {
    background-color: blue;
}
```

HTML:

```html
<div id="header">This is the header</div>
```

### **d. Universal Selector**

* Targets all elements on the page (`*`).

```css
* {
    margin: 0;
    padding: 0;
}
```

---

## **5. CSS Properties**

CSS properties control different aspects of how elements are displayed. Here are the main categories of properties:

### **a. Text and Font Properties**

* **color**: Sets the text color.
* **font-family**: Specifies the font of the text.
* **font-size**: Adjusts the size of the text.
* **font-weight**: Controls the thickness of the text (e.g., `normal`, `bold`).
* **line-height**: Controls the space between lines of text.
* **text-align**: Aligns text (e.g., `left`, `center`, `right`).

Example:

```css
p {
    color: darkblue;
    font-size: 18px;
    font-family: Arial, sans-serif;
    text-align: center;
}
```

### **b. Box Model (Layout) Properties**

The box model defines the layout of elements and includes padding, borders, margins, and the content area.

* **width**: Defines the width of an element.
* **height**: Defines the height of an element.
* **padding**: Space inside an element, between content and the border.
* **border**: The border surrounding the element.
* **margin**: Space outside an element, between it and other elements.

Example:

```css
div {
    width: 300px;
    height: 200px;
    padding: 20px;
    border: 2px solid black;
    margin: 10px;
}
```

### **c. Background Properties**

* **background-color**: Sets the background color.
* **background-image**: Adds an image as a background.
* **background-size**: Controls the size of the background image (e.g., `cover`, `contain`).

Example:

```css
body {
    background-color: #f0f0f0;
}

div {
    background-image: url('background.jpg');
    background-size: cover;
}
```

---

## **6. CSS Positioning**

CSS positioning properties allow you to control the position of elements.

### **a. Static (default)**:

Elements are positioned based on the normal flow of the document.

### **b. Relative**:

Positioned relative to its normal position.

```css
div {
    position: relative;
    top: 20px;
    left: 10px;
}
```

### **c. Absolute**:

Positioned relative to the nearest positioned ancestor (not static).

```css
div {
    position: absolute;
    top: 50px;
    left: 100px;
}
```

### **d. Fixed**:

Positioned relative to the viewport, so it stays in place when scrolling.

```css
div {
    position: fixed;
    top: 10px;
    left: 10px;
}
```

---

## **7. CSS Flexbox**

Flexbox is a layout model that provides an easy way to align and distribute space among items in a container.

```css
.container {
    display: flex;
    justify-content: space-between; /* Align items with space between them */
    align-items: center; /* Vertically align items */
}

.item {
    width: 100px;
    height: 100px;
    background-color: lightblue;
}
```

---

## **8. CSS Grid**

CSS Grid Layout is a two-dimensional layout system that allows you to create complex web designs more easily.

```css
.container {
    display: grid;
    grid-template-columns: repeat(3, 1fr); /* Creates 3 equal columns */
    gap: 10px; /* Adds space between grid items */
}

.item {
    background-color: lightcoral;
}
```

---

## **9. CSS Transitions and Animations**

CSS allows you to animate changes in properties.

### **a. Transitions**

Transitions allow property changes to occur over a specified duration.

```css
button {
    background-color: blue;
    color: white;
    transition: background-color 0.3s ease;
}

button:hover {
    background-color: red;
}
```

### **b. Animations**

Animations allow more complex keyframe-based animations.

```css
@keyframes move {
    from {
        transform: translateX(0);
    }
    to {
        transform: translateX(100px);
    }
}

div {
    animation: move 2s infinite alternate;
}
```

---

## **10. Responsive Design**

Responsive web design ensures that your site looks good on all screen sizes (desktops, tablets, and phones).

### **a. Media Queries**

Media queries allow you to apply different styles depending on the device’s screen size.

```css
@media (max-width: 768px) {
    body {
        background-color: lightblue;
    }
}
```

This will change the background color to `lightblue` if the screen width is 768px or smaller.

---

## **11. Conclusion**

CSS is a powerful tool that lets you control how HTML elements look and behave. With CSS, you can design complex layouts, add animations, and ensure your website looks good on any device. By learning about selectors, properties, and advanced layout techniques (like Flexbox and Grid), you can build modern, stylish websites.

# JS


## **1. What is JavaScript?**

* **JavaScript (JS)** is a programming language used to make web pages **interactive**.
* It can:

  * Respond to user actions (clicks, typing)
  * Change HTML content and CSS styles
  * Validate forms
  * Create animations and dynamic behavior
* JavaScript runs in the **browser**.

---

## **2. How to Add JavaScript to HTML**

### **a. Inline JavaScript**

* Written directly inside an HTML element (not recommended for large projects).

```html
<button onclick="alert('Hello!')">Click Me</button>
```

---

### **b. Internal JavaScript**

* Written inside a `<script>` tag in the HTML file.

```html
<script>
    alert("Hello from JavaScript!");
</script>
```

---

### **c. External JavaScript (Recommended)**

* Written in a separate `.js` file and linked to HTML.

```html
<script src="script.js"></script>
```

**script.js**

```javascript
alert("Hello from external JS!");
```

---

## **3. JavaScript Basics**

### **a. Variables**

Used to store data.

```javascript
let name = "John";     // Can be changed
const age = 20;       // Cannot be changed
var city = "London";  // Older way (avoid using)
```

---

### **b. Data Types**

Common JavaScript data types:

* **String** → `"Hello"`
* **Number** → `25`
* **Boolean** → `true` / `false`
* **Array** → `[1, 2, 3]`
* **Object** → `{ name: "John", age: 20 }`
* **Undefined** → variable with no value
* **Null** → empty value

Example:

```javascript
let message = "Hello";
let score = 100;
let isLoggedIn = true;
```

---

## **4. Operators**

### **a. Arithmetic Operators**

```javascript
let sum = 10 + 5;
let diff = 10 - 5;
let product = 10 * 5;
let quotient = 10 / 5;
```

### **b. Comparison Operators**

```javascript
5 == "5"    // true (loose comparison)
5 === "5"   // false (strict comparison)
5 != 3
5 > 3
```

### **c. Logical Operators**

```javascript
&&   // AND
||   // OR
!    // NOT
```

---

## **5. Conditional Statements**

Used to make decisions.

### **a. if / else**

```javascript
let age = 18;

if (age >= 18) {
    console.log("You are an adult");
} else {
    console.log("You are a minor");
}
```

---

### **b. switch Statement**

```javascript
let day = 2;

switch (day) {
    case 1:
        console.log("Monday");
        break;
    case 2:
        console.log("Tuesday");
        break;
    default:
        console.log("Unknown day");
}
```

---

## **6. Loops**

Used to repeat code.

### **a. for Loop**

```javascript
for (let i = 1; i <= 5; i++) {
    console.log(i);
}
```

### **b. while Loop**

```javascript
let i = 1;
while (i <= 5) {
    console.log(i);
    i++;
}
```

---

## **7. Functions**

Functions are reusable blocks of code.

```javascript
function greet(name) {
    return "Hello " + name;
}

console.log(greet("Alice"));
```

### **Arrow Function**

```javascript
const greet = (name) => {
    return "Hello " + name;
};
```

---

## **8. Events**

Events occur when users interact with the page.

Common events:

* `click`
* `mouseover`
* `keydown`
* `submit`

Example:

```html
<button id="btn">Click Me</button>

<script>
    document.getElementById("btn").addEventListener("click", function () {
        alert("Button clicked!");
    });
</script>
```

---

## **9. DOM Manipulation**

The **DOM (Document Object Model)** allows JavaScript to access and modify HTML elements.

### **a. Selecting Elements**

```javascript
document.getElementById("title");
document.querySelector(".box");
document.querySelectorAll("p");
```

---

### **b. Changing Content**

```javascript
document.getElementById("title").innerHTML = "New Title";
```

---

### **c. Changing Styles**

```javascript
document.getElementById("title").style.color = "red";
```

---

## **10. Arrays**

Used to store multiple values.

```javascript
let fruits = ["Apple", "Banana", "Mango"];

console.log(fruits[0]); // Apple
fruits.push("Orange"); // Add item
```

---

## **11. Objects**

Used to store related data.

```javascript
let person = {
    name: "John",
    age: 25,
    city: "New York"
};

console.log(person.name);
```

---

## **12. Form Validation Example**

```html
<input type="text" id="username">
<button onclick="check()">Submit</button>

<script>
function check() {
    let user = document.getElementById("username").value;
    if (user === "") {
        alert("Please enter username");
    } else {
        alert("Welcome " + user);
    }
}
</script>
```

---

## **13. Console**

The console is used for debugging.

```javascript
console.log("This is a message");
```

---

## **14. Conclusion**

* HTML = structure
* CSS = design
* **JavaScript = behavior**

JavaScript brings your website to life by adding logic, interactivity, and dynamic content.






