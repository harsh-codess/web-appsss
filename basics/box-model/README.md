# Box Model Project

## 📦 Understanding the CSS Box Model

The box model is the foundation of CSS layout. Every element is a box composed of:
1. **Content** - The actual content (text, images, etc.)
2. **Padding** - Space inside the border (transparent)
3. **Border** - The edge of the box
4. **Margin** - Space outside the border (transparent)

## 🎯 Visual Representation

```
┌─────────────────────────────────────────┐
│ Margin                                  │
│ ┌─────────────────────────────────────┐ │
│ │ Border                            │ │
│ │ ┌─────────────────────────────────┐ │ │
│ │ │ Padding                       │ │ │
│ │ │ ┌──────────────────────────────┐ │ │ │
│ │ │ │ Content                    │ │ │ │
│ │ │ └──────────────────────────────┘ │ │ │
│ │ │                                 │ │ │
│ │ └─────────────────────────────────┘ │ │
│ │                                     │ │
│ └─────────────────────────────────────┘ │
│                                         │
└─────────────────────────────────────────┘
```

## 🔢 Box Model Formula

```
Total Width = width + padding-left + padding-right + border-left + border-right + margin-left + margin-right
Total Height = height + padding-top + padding-bottom + border-top + border-bottom + margin-top + margin-bottom
```

## 💻 CSS Properties

### Padding (Inside)
```css
/* Sets space inside the border */
padding: 20px;           /* All sides */
padding: 10px 20px;      /* Vertical | Horizontal */
padding-top: 10px;       /* Individual sides */
```

### Border
```css
/* Creates an edge around padding */
border: 10px solid black;        /* Width | Style | Color */
border-top: 5px dashed red;      /* Individual sides */
```

### Margin (Outside)
```css
/* Sets space outside the border */
margin: 10px;            /* All sides */
margin: 10px auto;       /* Vertical | Horizontal (auto centers) */
margin-left: 20px;       /* Individual sides */
```

### Box Sizing
```css
/* Controls how width/height are calculated */
box-sizing: content-box;  /* Default (width = content only) */
box-sizing: border-box;   /* Modern approach (width = content + padding + border) */
```

## 📚 Project Guide

This project includes an element with:
- Width: 200px
- Height: 200px
- Padding: 20px
- Border: 10px solid black
- Background: cadetblue

**Total box width:** 200 + 20×2 + 10×2 = 260px
**Total box height:** 200 + 20×2 + 10×2 = 260px

## 🎨 CSS in This Project

```css
div { 
  height: 200px;           /* Content height */
  width: 200px;            /* Content width */
}

#first { 
  background-color: cadetblue;  /* Fill background */
  padding: 20px;                /* Internal spacing */
  border: 10px solid black;     /* Border around padding */
}
```

## 🔧 Exercises

Try modifying:
1. Increase `padding` and see the box grow
2. Change `border` color and style
3. Add `margin` to create space around elements
4. Use `box-sizing: border-box` to change width calculation

## 🖥️ Browser DevTools Tip

Open DevTools (F12) → Elements → select the div → look at the Box Model tab to see:
- Content area
- Padding area
- Border area
- Margin area

## 📖 References

- [MDN Box Model](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Box_Model)
- [Box Model Generator](https://www.cssportal.com/css-box-model/)
