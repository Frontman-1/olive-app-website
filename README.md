# 🫒 Olive App – Food Scanner Landing Page

A pixel-perfect, fully responsive landing page for **Olive** — a nutrition-focused mobile application that empowers families to make healthier grocery choices through instant barcode scanning and expert-backed food analysis.

---

## 🧠 About The Project

Olive is a food scanner app designed for health-conscious parents who want to eliminate harmful ingredients from their family's diet. This landing page serves as the app's primary marketing website, showcasing its features, pricing, testimonials, and value proposition in a clean, modern design.

The website is built from scratch using only **HTML5**, **CSS3**, **JavaScript**, and **Bootstrap 5** — no frameworks, no build tools, no dependencies beyond Bootstrap's CDN. Every section is hand-crafted with attention to micro-interactions, scroll-based reveal animations, and a cohesive olive-green design system.

### 🎯 What This Project Demonstrates

- Clean, semantic HTML5 with proper SEO meta tags and heading hierarchy
- A custom CSS design system using CSS custom properties (variables) for consistent theming
- Vanilla JavaScript for all interactivity — zero jQuery, zero external libraries
- Responsive design that adapts seamlessly across desktop, tablet, and mobile
- Modern UI patterns: glassmorphism navbar, infinite product sliders, FAQ accordion, scroll-triggered fade animations
- Professional-grade code organization and naming conventions

---

## 🛠️ Tech Stack

| Technology | Version | Role |
|:---|:---|:---|
| **HTML5** | — | Semantic structure, SEO, accessibility |
| **CSS3** | — | Custom properties, flexbox, grid, keyframe animations, glassmorphism |
| **JavaScript** | ES6+ | DOM manipulation, Intersection Observer API, event handling |
| **Bootstrap** | 5.3.3 | Responsive grid, utility classes, collapse component |

---

## 🔤 Typography & Fonts

| Font | Source | Weights Used | Purpose |
|:---|:---|:---|:---|
| **Inter** | Google Fonts | 300, 400, 450, 500, 600, 700, 800 | Primary typeface across all text |

Inter was chosen for its exceptional readability at all sizes, clean geometric forms, and extensive weight range — making it ideal for both crisp UI text and bold display headings.

---

## 🎨 Design System

### Color Palette

| Color | Hex Code | CSS Variable | Usage |
|:---|:---|:---|:---|
| 🟢 Primary Green | `#386641` | `--primary` | Buttons, headings, CTAs, navbar accents |
| 🟢 Primary Dark | `#2d5235` | `--primary-dark` | Hover states, pressed buttons |
| 🟡 Accent Yellow-Green | `#AEB93E` | `--accent` | Badges, highlights, newsletter button |
| ⬜ Light Background | `#F5FAF6` | `--bg-light` | Section backgrounds, cards |
| ⬛ Dark Text | `#1F3824` | `--text-dark` | Headings, primary body copy |
| 🔘 Muted Text | `#6b7280` | `--text-muted` | Descriptions, secondary text |

### Border Radius Tokens

| Token | Value | Used On |
|:---|:---|:---|
| `--radius-sm` | `0.5rem` | Small UI elements, nav links |
| `--radius-md` | `0.75rem` | FAQ items, mini product cards |
| `--radius-lg` | `1rem` | Step cards, testimonial cards |
| `--radius-xl` | `1.5rem` | Hero section, pricing cards, feature images |
| `--radius-full` | `9999px` | Buttons, avatars, pill shapes |

---

## 📐 Page Sections

### 1. Sticky Navbar
Glassmorphism effect with `backdrop-filter: blur(12px)`. Gains a subtle border and shadow on scroll via JavaScript class toggling. Includes logo, navigation links, sign-in link, and a primary CTA button.

### 2. Hero Section
Rounded container with a light green gradient background. Features trust-building avatar stack ("Trusted by thousands"), a bold headline, subtitle, iOS download button, and a phone mockup with an infinite-scrolling product slider behind it.

### 3. How It Works
Three-column grid explaining the app flow:
- **Scan & Detect** — Animated barcode scanner visual with a pulsing scan line
- **Data Analysis & Validation** — Infinite-scrolling product thumbnail carousel
- **Actionable Insights** — Recipe suggestion cards in a sliding carousel

### 4. Feature Highlights
Three alternating left-right layout blocks, each with an image and a bulleted feature list using green checkmark icons:
- Achieve Nutritional Clarity
- Proactive Ingredient Filtering
- Real Health Outcomes for Your Family

### 5. Testimonials
Three review cards on a light green background, each with 5-star ratings, quoted feedback, and reviewer avatars. Includes a link to 3,147+ App Store reviews.

### 6. Comparison Table
Dark green (`#386641`) section with a feature comparison grid — Olive vs. competitors. Uses green checkmarks and red crosses to visually communicate Olive's advantages.

### 7. Pricing Cards
Side-by-side Monthly and Yearly subscription cards. The yearly plan is highlighted with a "BEST VALUE" badge and a green border accent.

### 8. Independence Statement
Full-width section reinforcing Olive's credibility: *"100% Independent. Always."* — no brand deals, no affiliate links, no ads.

### 9. FAQ Accordion
Six expandable question-answer pairs. Built with vanilla JS — clicking a question smoothly reveals the answer via CSS `max-height` transitions. Only one item stays open at a time.

### 10. Final CTA
Bold dark green section with three feature callouts (effortless scanning, peace of mind, healthy recommendations) and a prominent white download button.

### 11. Footer
Three-column layout with tool links, about links, and a newsletter email subscription form. Bottom bar includes copyright notice and legal links (Terms, Privacy, Refund Policy).

---

## ⚡ Interactive Features

| Feature | How It Works |
|:---|:---|
| **Glassmorphism Navbar** | CSS `backdrop-filter: blur()` + JS scroll listener adds `.scrolled` class |
| **Scroll Reveal Animations** | Intersection Observer API triggers `.fade-up → .visible` CSS transitions |
| **Infinite Product Sliders** | JS clones slider content for seamless CSS `@keyframes` loop |
| **FAQ Accordion** | Click toggles `.active` class; CSS `max-height` handles smooth animation |
| **Barcode Scanner Animation** | CSS `@keyframes scanPulse` moves a highlight line up and down |
| **Newsletter Form** | JS form handler with email validation and success state feedback |
| **Smooth Anchor Scrolling** | JS calculates offset for navbar height and scrolls via `scrollTo()` |

---

## 📱 Responsive Design

| Viewport | Behavior |
|:---|:---|
| **≥ 992px** (Desktop) | Full multi-column layouts, side-by-side feature blocks |
| **768px – 991px** (Tablet) | Stacked feature blocks, adjusted comparison table padding |
| **< 768px** (Mobile) | Single-column layout, compact phone mockup, vertically stacked CTA features |

---

## 📁 Project Structure

```
olive-app-website/
├── index.html                       → Main landing page
├── favicon.ico                      → Browser tab icon
├── README.md                        → This file
├── css/
│   └── style.css                    → Design system + all custom styles
├── js/
│   └── script.js                    → All interactive functionality
└── assets/images/
    ├── olive.svg                    → Brand logo (SVG)
    ├── showcase.jpeg                → Feature section hero image
    ├── cta.png                      → Call-to-action visual
    ├── testimonials.png             → Testimonials section image
    ├── olive-faq.png                → FAQ section decoration
    ├── title.png                    → Section title decoration
    ├── benefits/
    │   ├── family.webp              → Family feature image
    │   └── hero-image.png           → Open Graph preview image
    ├── how-to/
    │   ├── barcode-image.png        → Barcode scanner visual
    │   └── slider/
    │       ├── product-1.png        → Product thumbnails (1–10)
    │       ├── ...
    │       ├── product-5-details.png→ Phone screen detail view
    │       └── straus-ice-cream.png → Featured product image
    └── testimonials/
        ├── meghan-l.png             → Reviewer avatar
        ├── tina-b.png               → Reviewer avatar
        └── lila-m.png               → Reviewer avatar
```

---

## 👤 Author

**Akhil R**

[![GitHub](https://img.shields.io/badge/GitHub-Frontman--1-181717?style=for-the-badge&logo=github)](https://github.com/Frontman-1)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-akhilpaila-0A66C2?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/akhilpaila/)

---

## 📄 License

This project is built for educational and portfolio demonstration purposes.

---

> Built with HTML5 · CSS3 · JavaScript · Bootstrap 5
