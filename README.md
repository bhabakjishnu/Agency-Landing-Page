# Agency Landing Page — Nexora Studio

A modern, responsive, accessible, and high-performance digital agency landing page built strictly with semantic **HTML5** and **Modern CSS3**—completely without JavaScript, CSS frameworks, or external runtime dependencies.

![Nexora Studio Desktop Preview](screenshots/desktop-preview.png)

---

## Overview

**Nexora Studio** is a fictional digital agency concept designed to reflect the aesthetic, architectural, and performance standards of modern 2026 web design. The landing page showcases end-to-end agency capabilities across brand strategy, UI/UX design, web architecture, and digital product engineering.

The project demonstrates how sophisticated visual hierarchy, glassmorphism, responsive data grids, fluid typography, and interactive micro-animations can be achieved using pure standards-compliant HTML and modern CSS.

---

## Project Objective

The primary objective of this capstone project is to demonstrate frontend engineering mastery without relying on frameworks, preprocessors, or JavaScript:

- Architecting an enterprise-grade, mobile-first design system with CSS Custom Properties.
- Implementing fluid responsive typography and spacing with mathematical CSS functions (`clamp()`, `min()`, `max()`, `minmax()`, and `calc()`).
- Building multi-dimensional asymmetric layouts with CSS Grid and flexible alignments with Flexbox.
- Achieving WCAG 2.1 AAA/AA accessibility compliance with visible keyboard `:focus-visible` indicators, semantic document structure, and screen-reader optimizations.
- Delivering sub-second render performance with zero JavaScript execution overhead and zero cumulative layout shift (CLS).

---

## Features

The landing page consists of 11 distinct, fully responsive sections:

1. **Header & Navigation**: Sticky blur header (`backdrop-filter`) with brand emblem, mobile-first horizontally scrollable navigation strip, and call-to-action button.
2. **Hero Section**: Eyebrow status pill with pulsing indicator, fluid clamp headline, value narrative, dual CTA touch targets, client impact metrics, and a pure-CSS interactive interface mockup with floating badges.
3. **Trust & Client Strip**: High-contrast, text-based branding strip featuring fictional partner organizations (`VORTEX LABS`, `LUMEN AI`, `SYNTHESIS`, `ORBITAL HQ`, `KINETIC`, `AURA VENTURES`).
4. **Services Section**: 6-card multi-column CSS Grid showcasing core agency capabilities, deliverable pills, and interactive hover transitions.
5. **Selected Work / Portfolio**: Asymmetric showcase of 3 flagship case studies (**AUREL**, **MONOFORM**, and **VERTEX**) featuring bespoke pure-CSS browser mockups, metrics tags, and category taxonomies.
6. **About & Agency Introduction**: Split-column manifesto highlighting the agency's philosophy alongside 4 foundational craft principles.
7. **Process Section**: 4-stage sequential workflow (`Discover`, `Define`, `Design`, `Deliver`) with an integrated connecting timeline on desktop.
8. **Statistics & Social Proof**: 4-column metric grid displaying agency milestones and awards with bold numerical hierarchy.
9. **Testimonials**: 3 genuine feedback reviews from verified client roles with star rating indicators and monogram avatar badges.
10. **Final Call to Action (CTA)**: High-impact conversion card with atmospheric radial glow, persuasive copy, and direct mail touchpoint.
11. **Footer**: Comprehensive semantic footer containing agency synopsis, navigation columns, capabilities directory, social media links with accessible inline SVGs, legal links, and smooth back-to-top navigation.

---

## Tech Stack

This project strictly adheres to native browser standards with zero external runtime dependencies:

- **Markup**: Semantic HTML5 (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, `<footer>`, `<figure>`, `<time>`)
- **Styling**: Modern CSS3 (Vanilla CSS)
- **Zero JavaScript**: 100% pure CSS interactions, responsive navigation, and transitions.
- **Zero Build Tools**: No npm, Vite, Webpack, Babel, Sass, or Tailwind required.
- **Typography**: Google Fonts (*Plus Jakarta Sans* & *JetBrains Mono*) with fallback to system fonts.
- **Icons**: Inline scalable vector graphics (SVG) with accessibility attributes (`aria-hidden="true"`).

---

## Project Structure

```
Agency-Landing-Page/
│
├── index.html                  # Semantic HTML5 single-page document
├── README.md                   # Project documentation
│
├── css/
│   └── style.css               # Mobile-first CSS architecture & design system
│
├── assets/
│   ├── images/
│   │   └── .gitkeep            # Reserved for raster assets (pure CSS mockups used)
│   └── icons/
│       └── .gitkeep            # Reserved for standalone icon assets (inline SVG used)
│
└── screenshots/
    ├── .gitkeep
    └── desktop-preview.png     # Full-fidelity desktop layout screenshot
```

---

## Design Highlights

- **Obsidian & Electric Indigo Aesthetic**: Deep luxury slate background (`#090a0f`) balanced with electric indigo (`#6366f1`), vivid violet (`#8b5cf6`), and cyber cyan (`#06b6d4`) highlights.
- **Glassmorphism & Depth**: Multi-layered card surfaces with 1px semi-transparent borders (`rgba(255, 255, 255, 0.08)`) and soft ambient radial glows.
- **Pure CSS Device Mockups**: Rather than relying on heavy external raster images, the interface features lightweight CSS-engineered browser chrome, metrics meters, chart bars, and code windows.
- **Micro-Interactions**: Subtle 2D transforms (`translateY`, `scale`) and smooth cubic-bezier easing curves on buttons, cards, and interactive links.

---

## Responsive Design

The stylesheet follows a strict **mobile-first** approach. Styles are authored starting with narrow viewports and expanded progressively using `min-width` media queries:

| Breakpoint | Target Devices | Layout Adjustments |
| :--- | :--- | :--- |
| **Base (<480px)** | Small & standard smartphones (320px–414px) | Single-column stack, full-width touch targets, horizontally scrollable nav strip |
| **480px** | Large phones & phablets | Inline button clusters, 2-column metrics |
| **768px** | Tablets & small iPads | 2-column service grid, 2-column work grid, 4-column stats, sticky desktop nav |
| **1024px** | Laptops & tablets in landscape | 3-column service grid, side-by-side featured work card, 4-column process timeline |
| **1280px+** | Standard & large desktop screens | Max container constraint (1240px) with auto margins, enlarged visual mockups |

### Tested Viewport Matrix
The layout has been tested with zero horizontal overflow across:
- `320px` (iPhone SE / small mobile)
- `360px` (Galaxy S8 / standard Android)
- `375px` (iPhone Mini / standard iOS)
- `390px` (iPhone 14/15)
- `414px` (iPhone Plus/Max)
- `480px` (Large mobile)
- `768px` (iPad Portrait)
- `820px` (iPad Air)
- `1024px` (iPad Pro / Small Laptop)
- `1280px` (Standard Desktop)
- `1440px` (MacBook Pro / High-res Desktop)
- `1920px` (Full HD 1080p Monitor)

---

## CSS Concepts Demonstrated

- **CSS Custom Properties**: Centralized `:root` design token architecture for colors, spacing, radii, shadows, and z-index layers.
- **Mathematical CSS Functions**:
  - `clamp()`: Fluid responsive headings (`font-size: clamp(2.25rem, 5vw + 1rem, 4.25rem);`) and fluid section padding.
  - `min()`: Container constraints (`width: min(100% - (var(--container-padding) * 2), var(--container-max-width));`).
  - `max()`: Boundary clamping for minimal tap target sizes.
  - `minmax()`: Responsive CSS Grid column sizing (`minmax(280px, 1fr)`).
  - `calc()`: Dynamic spacing and coordinate offsets.
- **CSS Logical Properties**: `margin-inline`, `padding-inline`, `margin-block`, `padding-block`, and `inset`.
- **CSS Flexbox**: 1D layout alignments for navigation, button clusters, tag clouds, trust strips, and metric rows.
- **CSS Grid**: 2D layout compositions for services, asymmetric portfolio showcases, process steps, and footer columns.
- **CSS Keyframe Animations & Transitions**:
  - `@keyframes heroFloat`: Subtle floating movement for the hero visual mockup.
  - `@keyframes pulseDot`: Live pulsating ambient indicator on status pills.
  - Hardware-accelerated 2D transforms (`translateY`, `scale`, `translateX`) using `cubic-bezier(0.4, 0, 0.2, 1)`.

---

## Accessibility

- **WCAG 2.1 Compliance**: High text contrast ratios meeting and exceeding AAA/AA standards (`#f8fafc` text on `#090a0f` background provides >18:1 contrast).
- **Keyboard Navigation**: Highly visible, high-contrast `:focus-visible` outline rings (`2px solid var(--color-accent-primary); outline-offset: 3px`) on all interactive controls.
- **Skip Link**: Accessible `<a href="#main-content" class="skip-link">Skip to main content</a>` positioned off-screen and revealed upon keyboard focus.
- **Semantic HTML Hierarchy**: Strict single `<h1>` tag with logically nested `<h2>`, `<h3>`, and `<h4>` subheadings.
- **Screen Reader Support**: Meaningful link labels, ARIA landmarks, `aria-hidden="true"` on decorative icons and visual mockups, and `role="list"` on unstyled lists.
- **Reduced Motion Support**:
  ```css
  @media (prefers-reduced-motion: reduce) {
    *, *::before, *::after {
      animation-duration: 0.01ms !important;
      transition-duration: 0.01ms !important;
      scroll-behavior: auto !important;
    }
  }
  ```

---

## Performance

- **Zero JavaScript Overhead**: No bundle parsing, execution pauses, or hydration delays.
- **Zero Layout Shift (CLS = 0)**: Explicit visual container dimensions and CSS aspect boundaries.
- **Optimized Assets**: Vector-only graphical composition and lightweight SVG emblems.
- **System Font Fallbacks**: Smooth font rendering with native system fallbacks if network connectivity is constrained.

---

## Getting Started

No build step or server setup is required.

### Option 1: Direct File Opening
Simply double-click `index.html` or open it directly in any modern browser:
```
file:///path/to/Agency-Landing-Page/index.html
```

### Option 2: Local Static Server (Optional)
If you prefer testing through a local web server:

Using Python:
```bash
python -m http.server 8080
```

Using Node (`npx`):
```bash
npx serve .
```

Then open `http://localhost:8080` in Google Chrome, Mozilla Firefox, Safari, or Microsoft Edge.

---

## Screenshots

```
screenshots/
└── desktop-preview.png
```

![Desktop Preview](screenshots/desktop-preview.png)

*To capture additional device viewports, run any headless browser utility and save screenshots directly into the `screenshots/` directory.*

---

## Future Improvements

- Dark/Light theme toggle using CSS Custom Properties with `:has()` or pure CSS checkbox state.
- Interactive contact form with client-side HTML5 validation constraints and styled pseudo-classes (`:valid`, `:invalid`, `:user-invalid`).
- View Transitions API integration for smooth page section transitions in supporting browsers.

---

## Learning Outcomes

- Mastery of modern CSS without relying on utility frameworks like Tailwind or component suites like Bootstrap.
- Practical experience structuring clean BEM-inspired CSS architectures capable of scaling across complex multi-section web properties.
- Deep comprehension of accessibility standards, screen-reader ergonomics, and mobile-first fluid layout systems.

---

## Author

Crafted as a professional capstone project for **Nexora Studio**.
License: MIT. Open for educational and portfolio demonstration use.
