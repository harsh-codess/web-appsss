# CSS Cascade Project

## 📖 Concept Overview

This project demonstrates the CSS Cascade, Specificity, and Inheritance - three core CSS concepts.

### What You'll Learn

**CSS Cascade**: When multiple styles apply to the same element, the browser determines which one wins.

**Specificity**: How CSS determines which style is most "important":
- ID selectors (highest): `#id`
- Class/Attribute selectors: `.class`, `[type="text"]`
- Element selectors (lowest): `div`, `p`

**Inheritance**: Some CSS properties are inherited from parent to child elements.

## 🎯 Project Structure

```
7-css-cascade/
├── index.html          # HTML structure (don't modify)
├── style.css           # Your exercise file
├── solution.css        # Reference solution
├── goal.png           # Target design
└── solution/
    ├── solution.html  # Alternative solution
    └── solution.css   # Alternative CSS solution
```

## 🔍 Exercise Tasks

1. **Understand the HTML structure**
   - Nested divs with different classes
   - Paragraphs with and without classes

2. **Apply styles to demonstrate cascade**
   - Style nested elements at different levels
   - Observe how specificity affects which style wins

3. **Test inheritance**
   - Set colors on parent elements
   - See which properties are inherited by children

## 💻 Key Concepts in This Project

### Specificity Wins
```css
/* Element selector (low specificity) */
p { color: yellow; }

/* Class selector (medium specificity) */
.white-text { color: white; }  /* This wins! */

/* ID selector (highest specificity) */
#outer-box { background-color: rgb(3, 1, 3); } /* This always wins */
```

### Inheritance
```css
/* Color is inherited */
div { color: blue; }
p { /* Color is blue (inherited) */ }

/* Padding is NOT inherited */
div { padding: 10px; }
p { /* Padding is 0 (not inherited) */ }
```

## 🚀 How to Use

1. Open `index.html` in VS Code
2. Use Live Server to preview changes
3. Modify `style.css` and see results update
4. Compare your work with `solution.css`

## ✨ Visual Guide

The project creates a series of nested boxes, each demonstrating:
- **Outer box**: Dark background (ID selector)
- **Middle boxes**: Blue background (class selector)
- **Inner boxes**: Red background (overrides cascade)
- **Text colors**: Yellow > White (class overrides element)

## 📝 Notes

- The HTML is locked and shouldn't be modified
- Focus entirely on CSS styling
- Use browser DevTools to inspect elements and see specificity
- Try removing styles progressively to understand cascade

## 🔗 Related Projects

- [Combining Selectors](../7.1-combining-selectors/) - Advanced selector techniques
- [CSS Basics](../basics/css-basics/) - Start here if new to CSS
