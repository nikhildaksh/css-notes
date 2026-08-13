# Lecture 3 — Border, Border Radius, Box Sizing + Width & Height

## Border
Borders add outline around elements.

```css
border: 2px solid black;
```

---

## Border Radius

Used to make rounded corners.

```css
border-radius: 10px;
border-radius: 50%;   /* circle */
```

---

## Width & Height

```css
width: 200px;
height: 100px;

width: 50%;     /* relative to parent */
width: 100vw;   /* full viewport width */
```

---

## Box Sizing

### content-box (default)
Width = only content size.  
Padding + border increase total size.

### border-box (recommended)
Width includes padding + border — total size stays fixed.

```css
box-sizing: border-box;
```

---

## Box Shadow

```css
/* box-shadow: x-offset  y-offset  blur  color; */
box-shadow: 5px 5px 10px black;
box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.3);
```

## Text Shadow

```css
/* text-shadow: x  y  blur  color; */
text-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
```

---

## Practice Task

Create a card with:

* border
* rounded corners
* fixed width/height
* box-sizing: border-box
* box-shadow
