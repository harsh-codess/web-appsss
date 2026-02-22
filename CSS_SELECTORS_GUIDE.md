# CSS Selectors Quick Reference

## Basic Selectors

| Selector | Example | Description |
|----------|---------|-------------|
| Element | `p { }` | Selects all `<p>` elements |
| Class | `.box { }` | Selects all elements with `class="box"` |
| ID | `#header { }` | Selects the element with `id="header"` |
| Universal | `* { }` | Selects all elements |

## Combining Selectors

### 1. Group Selector (,)
Applies same styles to multiple selectors.

```css
h1, h2, h3 {
  color: blue;
}
```

### 2. Descendant Selector (space)
Selects ALL nested elements regardless of depth.

```css
div p {
  /* Selects all <p> inside <div> */
}
```

### 3. Child Selector (>)
Selects ONLY direct children.

```css
div > p {
  /* Selects only <p> that are direct children of <div> */
}
```

### 4. Chained Selector (no space)
Element must match ALL conditions.

```css
p.highlighted {
  /* Selects <p> elements with class="highlighted" */
}

.box.active {
  /* Selects elements with BOTH "box" AND "active" classes */
}
```

### 5. Multiple Combiners
Combine different selector types for specificity.

```css
div.container > p.intro {
  /* Direct <p> children with "intro" class inside <div> with "container" class */
}
```

## Specificity

From highest to lowest:
1. Inline styles: `style="..."`
2. IDs: `#id`
3. Classes, attributes, pseudo-classes: `.class`, `[type="text"]`, `:hover`
4. Elements, pseudo-elements: `div`, `::before`

## Practice Tips

1. Start with simple selectors
2. Use browser DevTools to test selectors
3. Avoid over-specific selectors (keep it simple)
4. Use classes for reusable styles
5. Use IDs sparingly (mainly for JavaScript)

## Common Mistakes

❌ Don't: `div .box.active` (descendant + chained)
✅ Do: `div.box.active` (chained only)

❌ Don't: `#id #another-id` (too specific)
✅ Do: `.container .item` (use classes)

## Resources

- [MDN CSS Selectors](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Selectors)
- [CSS Specificity Calculator](https://specificity.keegan.st/)
