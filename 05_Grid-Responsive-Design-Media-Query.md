# Lecture 5 — Grid + Responsive Design + Media Query

## What is CSS Grid?
A 2D layout system for making complex designs easily.

```css
display: grid;
grid-template-columns: repeat(3, 1fr);   /* 3 equal columns */
gap: 20px;
```

---

## What is Responsive Design?

A webpage that adjusts automatically on:

* mobile
* tablet
* desktop

---

## Media Queries

Used to apply different CSS for different screen sizes.

```css
@media (max-width: 768px) {
  .box {
    width: 100%;
  }
}
```

---

## Common Screen Sizes

| Device     | Width   |
| ---------- | ------- |
| Mobile     | 320px   |
| Tablet     | 768px   |
| Laptop     | 1024px  |
| Widescreen | 1200px+ |

---

## Practice Task

* Create a 3-column grid
* Convert it to 1-column on mobile using media query
