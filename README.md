

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Features](#features)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [CSS Styling Steps](#css-styling-steps)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size
- See hover states for all interactive elements on the page
- Open a lightbox gallery by clicking on the large product image
- Switch the large product image by clicking on the small thumbnail images
- Add items to the cart
- View the cart and remove items from it

### Features

This e-commerce product page showcases a Fall Limited Edition Sneakers product with:

- **Responsive Design**: Optimized for mobile (375px), tablet (376px-768px), desktop (769px-1024px), and large screens (1025px+)
- **Product Gallery**: Main product image with thumbnail selector buttons
- **Dynamic Pricing**: Display of original price, discount percentage, and final price
- **Interactive Elements**: 
  - Add to cart functionality with quantity controls (increment/decrement)
  - Hover states on buttons and links
  - Cart icon and user profile menu
- **Navigation**: Comprehensive navbar with dropdown menu for mobile, full menu for desktop
- **Modern Styling**: Clean, professional design using custom CSS
- **Accessibility**: Semantic HTML with ARIA labels for screen reader support

### Links

- Solution URL: [E-Commerce Product Page](https://github.com/yourusername/ecommerce-product-page)
- Live Site URL: [View Live Demo](https://yourusername.github.io/ecommerce-product-page)

## My process

### Built with

- Semantic HTML5 markup
- CSS3 custom properties (variables)
- CSS Flexbox
- Mobile-first workflow
- Responsive design with media queries
- ARIA labels for accessibility
- Google Fonts (Kumbh Sans)

### CSS Styling Steps

The CSS implementation follows a structured, organized approach with 10 major sections:

#### 1. **Root & Base Styles**
- Global box-sizing model using `box-sizing: border-box`
- Font family: 'Kumbh Sans' for consistent typography
- Universal selector applies box-sizing to all elements including pseudo-elements
- Foundation for predictable and maintainable styling

#### 2. **Layout Container**
- Responsive container with `max-width: 1440px`
- Center alignment with `margin: 0 auto`
- Flexible padding (16px) ensures proper spacing on all devices

#### 3. **Header Section Styling**
- Navigation bar: Flexbox layout with gap-based spacing
- Logo: Responsive sizing with max-height constraint
- Navigation links: Centered alignment with proper spacing and color (`hsl(219, 9%, 45%)`)
- Header images: Cart and avatar icons with fixed dimensions
- Divider: Subtle border separating header from content

#### 4. **Hero Section - Image Gallery**
- Main image: Full-width responsive with 8px border-radius
- Thumbnails: Flexbox layout with 1.5rem gap spacing
- Individual thumbnail buttons: 60px × 60px with object-fit
- Interactive buttons with cursor pointer indication

#### 5. **Hero Section - Product Content**
- Pretitle: Small uppercase text with letter-spacing
- Product title: Large heading (1.75rem) for prominence
- Description: Readable text with proper color contrast
- Price display: Flexbox alignment with multiple price elements
- Discount badge: Dark background with white text on orange accent

#### 6. **Cart Controls Section**
- Quantity selector: Light gray background (`hsl(0, 8%, 95%)`)
- Plus/minus buttons: Minimal styling with pointer cursor
- Tally value: Bold, centered display
- Add to cart button: Orange CTA (`hsl(26, 100%, 55%)`) with full-width mobile layout

#### 7. **Color Palette**
```css
Primary Orange (CTA): hsl(26, 100%, 55%)
Dark Text: hsl(0, 0%, 0%)
Secondary Gray: hsl(219, 9%, 45%)
Light Background: hsl(0, 8%, 95%)
Divider Gray: #e1e1e1
```

#### 8. **Responsive Breakpoints**

**Mobile (≤375px):**
- Reduced font sizes (title: 1.25rem, price: 1rem)
- Tighter thumbnail spacing (0.75rem)
- Optimized button padding and sizing
- Smaller logo max-height (16px)

**Tablet (376px - 768px):**
- Navigation links hidden with dropdown menu
- Hero section padding: 1.5rem 0
- Adjusted cart controls spacing

**Large Tablet (769px - 1024px):**
- Navigation links displayed
- Hero layout: Horizontal with flex-direction row
- Increased padding and spacing (2rem 4rem)
- Thumbnail size: 72px × 72px
- Add to cart minimum width: 200px

**Desktop (1025px+):**
- Maximum spacing and layout optimization
- Header bar uses space-between justification
- Hero gap: 5rem for breathing room
- Hero section padding: 2rem 10rem
- Add to cart minimum width: 220px

#### 9. **Interactive Elements & Accessibility**
- Buttons: Removed default browser styling (`border: none`, `background: none`)
- Cursor states: `cursor: pointer` on interactive elements
- ARIA labels for screen readers: `aria-label="Add to cart"`
- Semantic HTML: `<nav>`, `<section>`, `<button>` tags
- Role attributes: `role="region"`, `role="group"` for enhanced accessibility
- Color contrast meets WCAG standards

#### 10. **Spacing System**
Uses consistent rem-based spacing scale: 0.5rem, 0.75rem, 1rem, 1.5rem, 2rem, 3rem, 5rem, 10rem
Ensures scalable, maintainable, and proportional spacing throughout

### What I learned

Through building this project, I strengthened my understanding of:

```css
/* Flexbox alignment patterns */
.navbar {
  display: flex;
  align-items: center;
  justify-content: flex-start;
  gap: 1rem;
}

/* Responsive typography using rem units */
.product-title {
  font-size: 1.75rem; /* Scales with base font size */
}

/* Mobile-first media query approach */
@media (min-width: 769px) {
  .hero {
    flex-direction: row;
    gap: 3rem;
  }
}
```

Key takeaways:
- Mobile-first approach simplifies responsive design
- CSS custom properties (HSL colors) improve maintainability
- Flexbox provides powerful layout control without JavaScript
- Proper semantic HTML and ARIA labels improve accessibility
- Organized CSS structure with clear comments aids future maintenance

### Continued development

Areas to focus on in future projects:
- Implementing JavaScript functionality for interactive features (lightbox gallery, cart functionality)
- Adding CSS animations and transitions for smooth interactions
- Exploring CSS Grid for complex multi-column layouts
- Implementing dark mode with CSS variables
- Performance optimization with lazy loading for images
- Progressive enhancement with feature detection

### Useful resources

- [MDN Web Docs - Flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout) - Essential reference for layout techniques
- [CSS Tricks - A Complete Guide to Grid](https://css-tricks.com/snippets/css/complete-guide-grid/) - Advanced layout patterns
- [Web.dev - Responsive Design](https://web.dev/responsive-web-design-basics/) - Mobile-first principles
- [WCAG Accessibility Guidelines](https://www.w3.org/WAI/WCAG21/quickref/) - Accessibility standards and practices
- [Google Fonts - Kumbh Sans](https://fonts.google.com/specimen/Kumbh+Sans) - Typography resource

## Author

- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)
- GitHub - [@yourusername](https://github.com/yourusername)
- Portfolio - [Your website](https://yourwebsite.com)
