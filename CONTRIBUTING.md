# Contributing to Web Development Projects

Thank you for your interest in contributing to this learning repository!

## 📋 Project Guidelines

### HTML Standards
- Use semantic HTML5 elements where appropriate
- Always include proper meta tags (charset, viewport)
- Use descriptive class and ID names
- Keep HTML structure clean and simple

### CSS Best Practices
- Follow a consistent naming convention for classes
- Group related properties together
- Use meaningful class names (e.g., `.button-primary` not `.btn1`)
- Comment complex selectors or properties
- Avoid inline styles - use external stylesheets

### Code Style

```html
<!-- Good -->
<div class="container">
  <header class="header-main">
    <h1>Title</h1>
  </header>
</div>

<!-- Avoid -->
<div class="c">
  <h1 style="color: red;">Title</h1>
</div>
```

```css
/* Group related properties */
.button {
  /* Layout */
  display: inline-block;
  padding: 10px 20px;
  margin: 5px;
  
  /* Colors */
  background-color: blue;
  color: white;
}
```

## 🔄 Workflow

1. Create a new branch for your changes
   ```bash
   git checkout -b feature/project-name
   ```

2. Make your changes with clear commit messages
   ```bash
   git commit -m "feat: add styling to box-model project"
   ```

3. Push your branch and create a pull request

## 💡 Learning Path

1. **Start with basics/** - Master fundamental concepts
2. **Progress to 7-css-cascade/** - Understand specificity and inheritance
3. **Practice 7.1-combining-selectors/** - Advanced selector techniques

## 📚 Helpful Resources

- [MDN Web Docs - CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [CSS Selectors Reference](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Selectors)
- [HTML5 Semantic Elements](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)

## ✅ Before Committing

- [ ] HTML is valid
- [ ] CSS is properly formatted
- [ ] No inline styles
- [ ] Meaningful commit messages
- [ ] Comments added for complex code

---

Happy learning! 🎓
