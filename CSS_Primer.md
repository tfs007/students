
# **CSS Primer Handout**

## **1. What is CSS?**

CSS (Cascading Style Sheets) is a stylesheet language used to define the visual presentation of HTML elements.

---

## **2. CSS Syntax**

```css
selector {
  property: value;
}
```

* `selector`: Targets the HTML element
* `property`: The style attribute (e.g., `color`)
* `value`: The setting for the property (e.g., `blue`)

Example:

```css
p {
  color: blue;
  font-size: 18px;
}
```

---

## **3. Applying CSS**

### a. Inline

```html
<p style="color: red;">Text</p>
```

### b. Internal

```html
<head>
  <style>
    p { color: red; }
  </style>
</head>
```

### c. External (Recommended)

```html
<link rel="stylesheet" href="style.css">
```

---

## **4. Selectors**

| Selector Type | Syntax          | Description                  |
| ------------- | --------------- | ---------------------------- |
| Element       | `p {}`          | All `<p>` elements           |
| Class         | `.className {}` | All elements with that class |
| ID            | `#idName {}`    | The element with that ID     |
| Universal     | `* {}`          | All elements                 |

---

## **5. Text Styling Properties**

```css
h1 {
  color: #333333;
  font-family: Arial, sans-serif;
  font-size: 24px;
  text-align: center;
  font-style: italic;
}
```

---

## **6. Color Values**

* Named: `red`, `blue`, `orange`
* Hexadecimal: `#ff5733`
* RGB: `rgb(255, 0, 0)`
* HSL: `hsl(0, 100%, 50%)`

---

## **7. Box Model**

```css
div {
  padding: 10px;
  margin: 20px;
  border: 2px solid black;
}
```

* `padding`: Space inside the element
* `margin`: Space outside the element
* `border`: Line around the element

---

## **8. Flexbox Layout**

```css
.container {
  display: flex;
  justify-content: space-around;
  align-items: center;
}
```

* `display: flex`: Enables flex layout
* `justify-content`: Horizontal alignment
* `align-items`: Vertical alignment

---

## **9. Pseudo-Class Example**

```css
button:hover {
  background-color: green;
  color: white;
}
```

* `:hover` applies the style when the user hovers over the element

---

## **10. Media Queries (Responsive Design)**

```css
@media (max-width: 600px) {
  body {
    background-color: lightgray;
  }
}
```

Applies styles only when the screen width is 600px or less.

---

## **11. Example: HTML + Internal CSS**

```html
<!DOCTYPE html>
<html>
<head>
  <title>CSS Primer</title>
  <style>
    body {
      background-color: #f0f0f0;
      font-family: sans-serif;
      color: #333;
    }
    h1 {
      color: navy;
      text-align: center;
    }
    .box {
      background-color: #fafad2;
      border: 2px dashed orange;
      padding: 20px;
      width: 300px;
      margin: 20px auto;
    }
  </style>
</head>
<body>
  <h1>CSS Primer Example</h1>
  <div class="box">
    <p>This is a styled box using CSS.</p>
  </div>
</body>
</html>
```

---


