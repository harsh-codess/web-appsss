# CSS Basics Project

## 🎨 Introduction to CSS

CSS (Cascading Style Sheets) is used to style HTML elements and control their appearance.

### Three Ways to Add CSS

```html
<!-- 1. External Stylesheet (Best Practice) -->
<link rel="stylesheet" href="style.css">

<!-- 2. Internal Style Tag -->
<style>
  p { color: blue; }
</style>

<!-- 3. Inline (Avoid) -->
<p style="color: blue;">Text</p>
```

## 🔷 CSS Syntax

```css
selector {
  property: value;
  property: value;
}
```

### Example
```css
p {
  color: blue;
  font-size: 16px;
  margin: 10px;
}
```

## 🎯 Basic Selectors

| Selector | Example | Targets |
|----------|---------|---------|
| Element | `p { }` | All `<p>` elements |
| Class | `.highlight { }` | Elements with `class="highlight"` |
| ID | `#header { }` | Element with `id="header"` (unique) |
| Universal | `* { }` | ALL elements |

## 🌈 Common Properties

### Text Properties
```css
color: red;                    /* Text color */
font-size: 16px;              /* Text size */
font-family: Arial, sans-serif; /* Font type */
text-align: center;           /* Left, center, right, justify */
font-weight: bold;            /* Weight: normal, bold, 100-900 */
```

### Box Properties
```css
background-color: lightblue;  /* Background fill */
padding: 10px;                /* Internal spacing */
margin: 10px;                 /* External spacing */
border: 1px solid black;      /* Edge around element */
width: 200px;                 /* Element width */
height: 100px;                /* Element height */
```

### Display Properties
```css
display: block;               /* Full width block */
display: inline;              /* Inline with text */
display: inline-block;        /* Inline but respects width/height */
display: flex;                /* Flexible layout */
display: none;                /* Hidden */
```

## 🎓 Best Practices

✅ **DO:**
- Use external stylesheets
- Use classes for reusable styles
- Use meaningful names (`.button-primary` not `.b1`)
- Keep related properties together
- Add comments for clarity

❌ **DON'T:**
- Use inline styles
- Overuse IDs for styling
- Use vague class names
- Style too specifically
- Forget about performance

## 🔗 CSS in Action

```css
/* Style all paragraphs */
p {
  font-size: 16px;
  line-height: 1.5;
}

/* Style specific paragraph */
.intro {
  color: #333;
  font-weight: bold;
}

/* Hover effect */
.button:hover {
  background-color: darkblue;
}
```

## 📚 Learning Path

1. Master basic selectors and properties
2. Understand box model (padding, margin, border)
3. Learn layout (display, flexbox, grid)
4. Practice cascade and specificity
5. Explore advanced CSS (animations, transforms)

## 🚀 Next Steps

After mastering CSS basics, learn:
- [Box Model](../box-model/) - Spacing and sizing
- [Fonts](../fonts/) - Typography
- [Cascade & Specificity](../../7-css-cascade/) - How CSS decides which styles apply
- [Selectors](../../7.1-combining-selectors/) - Advanced selector techniques

## 📖 Resources

- [MDN CSS Reference](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [CSS Tricks](https://css-tricks.com/)
- [W3C CSS Specification](https://www.w3.org/)
