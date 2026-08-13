# Lecture 6 — Display, Position, Hover, Transition + Mini Project

## Display Property

```css
display: block;         /* full width, new line */
display: inline;        /* only takes content width, no width/height */
display: inline-block;  /* inline but width/height works */
```

---

## Position Property

Used to place elements anywhere.

```css
position: static;    /* default */
position: relative;  /* relative to its normal position */
position: absolute;  /* relative to nearest positioned parent */
position: fixed;     /* fixed on screen, doesn't scroll */
position: sticky;    /* relative until scroll point, then fixed */
```

Example:

```css
position: absolute;
top: 20px;
left: 30px;
```

---

## Hover Effect

```css
button:hover {
  background: black;
  color: white;
}
```

---

## Transition

Smooth animation effect on property change.

```css
transition: 0.3s;
transition: all 0.3s ease;
```

---

## Overflow

```css
overflow: hidden;    /* hides content that overflows */
overflow: scroll;    /* adds scrollbar */
overflow: auto;      /* scrollbar only when needed */
```

---

## Mini Project (1 Hour)

Build a small **Landing Page**:

* Header
* Navigation bar
* Hero section
* Cards (Grid/Flex)
* Footer
* Fully responsive

This will combine everything learned from Lecture 1 to Lecture 6.
