# Frontend Mentor - Recipe page

![Design preview for the Recipe page coding challenge](./preview.jpg)

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My Process](#my-process)
  - [Built With](#built-with)
  - [What I Learned](#what-i-learned)
  - [Continued Development](#continued-development)
  - [Useful Resources](#useful-resources)
- [Author](#author)

## Overview

This is a solution to the [Recipe page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/recipe-page-KiTsR8QQKm). The challenge focuses on creating a responsive recipe card component with proper typography, spacing, and mobile-first design principles.

### Screenshot

#### 📱 Mobile View  
<img width="367" height="750" alt="Mobile view of recipe page" src="https://github.com/user-attachments/assets/2ec4cce4-70c8-4623-9eb4-d37d1885bf1e" />

#### 💻 Desktop View  
<img width="1875" height="945" alt="Desktop view of recipe page" src="https://github.com/user-attachments/assets/581ced28-40f7-4dc3-82a2-502c194a4ba8" />

### Links

- **Solution URL:** [https://github.com/Raizo-03/recipe-page](https://github.com/Raizo-03/recipe-page)
- **Live Site URL:** [https://recipe-page-omelette.vercel.app](https://recipe-page-omelette.vercel.app)

## My Process

### Built With

- Semantic HTML5 markup
- CSS custom properties (CSS variables)
- Flexbox for layout and alignment
- Responsive units: `rem`, `em`, `px`, `%`, `vh`, `vw`
- BEM methodology for CSS naming
- Media queries (mobile-first approach)
- CSS border-radius and box-shadow
- Typography scaling with responsive units
- HTML tables for nutrition data

### What I Learned

This project was a **deep dive into Flexbox and responsive units**, providing valuable insights into modern CSS layout techniques and UI design principles:

#### 🎯 **Flexbox Mastery**
- **Container alignment**: Used `align-items: center` and `justify-content: center` for perfect centering
- **Responsive behavior**: Learned how `align-items: stretch` fills mobile viewports completely
- **Flex direction control**: Implemented `flex-direction: column` for vertical stacking
- **Self-alignment**: Applied `align-self: flex-start` for precise element positioning

```css
/* Key Flexbox insight: Mobile full-width containers */
@media (max-width: 768px) {
    body {
        align-items: stretch; /* Fills entire viewport width */
    }
    
    .container {
        width: 100%;
        border-radius: 0; /* Prevents visual gaps from rounded corners */
    }
}
```

#### 📐 **Responsive Units Deep Dive**
- **`rem` vs `em`**: Used `rem` for consistent sizing, `em` for component-relative scaling
- **Percentage units**: Applied `%` for fluid image sizing and container widths
- **Viewport units**: Leveraged `vh` for minimum height constraints
- **Pixel precision**: Used `px` for borders and fine details where exact control was needed

```css
/* Responsive unit strategy */
.container-header_title {
    font-size: 2rem;        /* Scalable with root font-size */
    padding: 1rem 2rem;     /* Consistent spacing */
}

.container-header_image {
    width: 100%;            /* Fluid responsive image */
    height: auto;           /* Maintains aspect ratio */
}
```

#### 🎨 **UI Design Insights**
- **Border-radius behavior**: Discovered how rounded corners create visual gaps on mobile
- **Table styling**: Mastered `border-collapse: collapse` for seamless table borders
- **Typography hierarchy**: Implemented proper font-weight and size relationships
- **Visual rhythm**: Created consistent spacing patterns using CSS custom properties

```css
/* UI insight: Border opacity for subtle dividers */
.container-nutrition_table th,
.container-nutrition_table td {
    border-bottom: 1px solid rgba(200, 200, 200, 0.4);
}
```

#### 🔧 **CSS Architecture Lessons**
- **BEM methodology**: Structured CSS with `.block__element--modifier` pattern
- **CSS custom properties**: Implemented design token system with `--stone-300`, `--white`
- **Mobile-first approach**: Built responsive design from smallest screen up
- **Semantic HTML**: Used proper heading hierarchy and table structure

### Continued Development

For future projects, I plan to focus on:

- **CSS Grid mastery**: Complex two-dimensional layouts
- **Container queries**: Element-based responsive design
- **Advanced Flexbox**: Nested flex containers and complex alignment
- **CSS `clamp()`**: Fluid typography and spacing
- **Accessibility**: ARIA labels, focus management, screen reader optimization
- **Performance**: Critical CSS, font loading strategies, image optimization
- **Modern CSS**: Logical properties, aspect-ratio, CSS nesting

### Useful Resources

- [CSS Tricks - A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) - Essential flexbox reference
- [MDN Web Docs - CSS Flexible Box Layout](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout) - Comprehensive flexbox documentation
- [CSS Units Guide – CSS Tricks](https://css-tricks.com/the-lengths-of-css/) - Deep dive into responsive units
- [BEM Methodology](https://getbem.com/) - CSS naming convention guide
- [MDN Media Queries](https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries) - Responsive design techniques
- [CSS Custom Properties Guide](https://css-tricks.com/a-complete-guide-to-custom-properties/) - CSS variables mastery
- [Every Layout](https://every-layout.dev/) - Modern CSS layout patterns

## Author

- GitHub – [@Raizo-03](https://github.com/Raizo-03)
- Frontend Mentor – [@Raizo-03](https://www.frontendmentor.io/profile/Raizo-03)