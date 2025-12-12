# Blog Preview Card

A responsive blog preview card built as part of the [Frontend Mentor](https://www.frontendmentor.io/challenges/blog-preview-card-ckPaj01IcS) challenge.

## Overview

This project showcases a modern blog card designed with hover effects, fluid typography, and accessible semantic markup.

### Screenshot

![Blog Preview Card](./assets/images/solution.png)

### Links

- Solution URL: [GitHub Repository](https://github.com/hakan-kemal/blog-preview-card)
- Live Site URL: [Netlify Deployment](https://blog-preview-card-hk.netlify.app/)

## My Process

### Built With

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow
- Fluid typography using `clamp()`
- [Figtree](./assets/fonts/) - Google Font (local files)

### What I Learned

This project helped me explore several interesting CSS concepts:

**Fluid Typography with clamp():**

```css
:root {
  --fs-small: clamp(12px, 3.2vw, 14px);
  --fs-medium: clamp(14px, 3.73vw, 16px);
  --fs-large: clamp(20px, 5.33vw, 24px);
}
```

Using `clamp()` for font sizes creates truly responsive typography that scales smoothly between mobile and desktop without media queries.

**CSS Custom Properties for Design Tokens:** Organized colors and sizing into reusable CSS variables for maintainability:

```css
:root {
  --yellow: hsl(47, 88%, 63%);
  --gray-950: hsl(0, 0%, 7%);
}
```

**Modern CSS Nesting:** Utilized native CSS nesting for hover states, keeping related styles together:

```css
.title-link {
  color: var(--gray-950);

  &:hover,
  &:focus {
    color: var(--yellow);
  }
}
```

**Box Shadow Effects:** Created a bold, modern card design with offset shadows:

```css
.card {
  box-shadow: 8px 8px 0 rgba(0, 0, 0, 1);
  border: 1px solid var(--gray-950);
}
```

### Continued Development

Areas I want to focus on in future projects:

- Advanced CSS animations and transitions
- CSS Grid for more complex layouts
- Dark mode implementation with CSS variables
- Enhanced accessibility features (ARIA labels, keyboard navigation)

### Useful Resources

- [MDN Web Docs - clamp()](https://developer.mozilla.org/en-US/docs/Web/CSS/clamp) - Excellent guide on fluid typography
- [CSS-Tricks - CSS Nesting](https://css-tricks.com/css-nesting/) - Understanding native CSS nesting
- [Google Fonts](https://fonts.google.com/) - Font selection and optimization

## Author

- Frontend Mentor - [@hakan-kemal](https://www.frontendmentor.io/profile/hakan-kemal)
- GitHub - [@hakan-kemal](https://github.com/hakan-kemal)

## Acknowledgments

Thanks to Frontend Mentor for providing this challenge and the design specifications.
