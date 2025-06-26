# CSS Concepts

## What is CSS?

**CSS** stands for **Cascading Style Sheets**. It is a stylesheet language used to describe the presentation (look and formatting) of a document written in HTML or XML. CSS controls the layout, colors, fonts, and overall visual appearance of web pages.

---

## Core CSS Concepts

### 1. Selectors
Selectors are patterns used to select the HTML elements you want to style.
```css
/* Selects all <p> elements */
p {
  color: blue;
}
```

### 2. Properties and Values
Properties define which aspect of the element you want to style (e.g., color, font-size), and values determine how it will appear.
```css
h1 {
  font-size: 2em;
  color: red;
}
```

### 3. Classes and IDs
- **Class:** Can be used on multiple elements. Prefixed with a `.` in CSS.
- **ID:** Should be unique in a document. Prefixed with `#` in CSS.

```css
.my-class {
  background-color: yellow;
}
#unique-id {
  border: 1px solid black;
}
```

### 4. The Box Model

Every HTML element is considered a rectangular box, consisting of:

- **Content:** The actual text or image.
- **Padding:** Clears an area around the content (inside the border).
- **Border:** Surrounds the padding and content.
- **Margin:** Clears an area outside the border (space between elements).

```css
div {
  margin: 10px;         /* Space outside the border */
  padding: 20px;        /* Space between content and border */
  border: 2px solid gray;
}
```

### 5. Padding

**Padding** is the space between the content of an element and its border. You can set it for all sides or individually:

```css
/* All sides */
.box {
  padding: 20px;
}
/* Top, Right, Bottom, Left */
.box {
  padding: 10px 15px 20px 25px; /* top right bottom left */
}
/* Individual sides */
.box {
  padding-top: 10px;
  padding-right: 15px;
  padding-bottom: 20px;
  padding-left: 25px;
}
```

### 6. Margin

**Margin** is the space outside the border of an element, creating space between elements.

```css
.box {
  margin: 10px 20px; /* top-bottom right-left */
}
```

### 7. Positioning

Controls how elements are placed on the page:
- `static` (default)
- `relative`
- `absolute`
- `fixed`
- `sticky`

```css
.relative-box {
  position: relative;
  top: 10px;
  left: 20px;
}
```

### 8. Flexbox

A modern layout mode for aligning items in rows or columns.

```css
.container {
  display: flex;
  justify-content: center;
  align-items: center;
}
```

### 9. Grid

A two-dimensional layout system for complex designs.

```css
.grid-container {
  display: grid;
  grid-template-columns: 1fr 2fr;
  gap: 10px;
}
```

### 10. Responsive Design

Make your website look good on all devices with media queries.

```css
@media (max-width: 600px) {
  body {
    background-color: lightblue;
  }
}
```

### 11. Pseudo-classes and Pseudo-elements

Special effects when elements are in a certain state or to style parts of elements.

```css
a:hover {
  color: green;
}
p::first-line {
  font-weight: bold;
}
```

### 12. Transitions and Animations

Add smooth effects and animations.

```css
.box {
  transition: background-color 0.5s;
}
@keyframes example {
  from {background-color: red;}
  to {background-color: yellow;}
}
```

---

## Learn More

- [MDN Web Docs: CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [W3Schools: CSS Tutorial](https://www.w3schools.com/css/)

Feel free to contribute more CSS concepts!
