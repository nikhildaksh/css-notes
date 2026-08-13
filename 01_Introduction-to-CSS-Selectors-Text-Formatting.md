# Lecture 1 — Introduction to CSS + Selectors + Text Formatting

## What is CSS?
CSS stands for **Cascading Style Sheets**.  
It is used to style and design web pages.

With CSS, we can change:
- colors  
- sizes  
- layouts  
- spacing  
- fonts  

HTML creates the structure.  
CSS makes it look beautiful.

---

## Types of CSS

### 1. Inline CSS
```html
<p style="color:red;">Hello</p>
```

### 2. Internal CSS

```html
<style>
p { color: blue; }
</style>
```

### 3. External CSS (Recommended)

```html
<link rel="stylesheet" href="style.css">
```

---

## CSS Selectors

### 1. Element Selector
Selects all tags of one type.

```css
p {
  color: red;
}
```

### 2. Class Selector
Used for reusable styling.

```css
.title {
  font-size: 24px;
}
```

### 3. ID Selector
Used for unique element.

```css
#main {
  color: green;
}
```

---

## Text Formatting Properties

```css
color: red;                     /* Text color */
font-size: 24px;                /* Text size */
text-decoration: underline;     /* Underline, none, etc */
text-align: center;             /* left, right, center */
font-weight: bold;              /* bold, normal, 100-900 */
```

---

## Practice Task

* Create headings & paragraphs
* Apply colors & sizes
* Try ID, class, and element selectors
