# Lecture 7 — Transition & Animation

## Transition

Transition makes a property change **smooth** instead of instant.

It requires a trigger like `:hover`, `:focus`, or `:active`.

### Syntax

```css
transition: property  duration  timing-function  delay;
```

### Example

```css
.box {
    transition: all 0.3s ease;
}

.box:hover {
    background: black;
}
```

---

## Timing Functions

Controls the speed pattern of the transition.

| Function     | Behavior                     |
| ------------ | ---------------------------- |
| linear       | Same speed throughout        |
| ease         | Slow → Fast → Slow (default) |
| ease-in      | Starts slow                  |
| ease-out     | Ends slow                    |
| ease-in-out  | Starts and ends slow         |

```css
transition: all 2s linear;
transition: all 2s ease;
transition: all 2s ease-in;
transition: all 2s ease-out;
transition: all 2s ease-in-out;
```

---

## Delay

```css
/* transition: property  animation-time  delay; */
transition: all 1s 2s;   /* wait 2s, then animate for 1s */
```

---

## Animation

Transition needs a trigger to run.  
**Animation runs on its own — no trigger needed.**

Examples: loading spinner, bouncing ball, rotating icon.

---

## Animation — Step 1: Define @keyframes

```css
@keyframes move {
    from { left: 0; }
    to   { left: 300px; }
}
```

Or using percentages:

```css
@keyframes move {
    0%   { left: 0; }
    100% { left: 300px; }
}
```

---

## Animation — Step 2: Apply It

```css
/* animation: name  duration  timing-function  delay  iteration-count  direction  fill-mode; */

.box {
    animation: move 2s ease 0s 1 normal forwards;
}
```

---

## Animation Properties

```css
animation-name: move;                /* Which animation to run */
animation-duration: 2s;              /* How long it takes to complete */
animation-delay: 1s;                 /* Wait before starting */
animation-timing-function: ease;     /* Speed pattern */
animation-iteration-count: 3;        /* How many times it runs */
animation-iteration-count: infinite; /* Runs forever */
animation-direction: normal;         /* Which direction it plays */
animation-fill-mode: forwards;       /* State after animation ends */
```

---

## animation-direction

```css
animation-direction: normal;            /* Start → End */
animation-direction: reverse;           /* End → Start */
animation-direction: alternate;         /* Start→End, End→Start, ... */
animation-direction: alternate-reverse; /* End→Start, Start→End, ... */
```

---

## animation-fill-mode

```css
animation-fill-mode: none;      /* Default — returns to original state */
animation-fill-mode: forwards;  /* Stays at the last keyframe state */
```

---

## Quick Reference

| Property        | Think of it as...                  |
| --------------- | ---------------------------------- |
| @keyframes      | Script of the movie                |
| animation-name  | Name of the movie                  |
| duration        | How long the movie runs            |
| delay           | How long before the movie starts   |
| iteration-count | How many times the movie repeats   |
| direction       | Play forward or in reverse         |
| fill-mode       | Pause on last scene or reset       |

---

## Practice Task

* Create a box that smoothly changes color on hover (transition)
* Create a box that moves left to right on its own (animation)
* Build a loading spinner using `animation-iteration-count: infinite`
