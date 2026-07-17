# Frontend Mentor - Huddle landing page with single introductory section solution

Huddle Landing Page - This small project builds out a landing page with a single introductory section with Semantic HTML and CSS.

This is a solution to the [Huddle landing page with single introductory section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/huddle-landing-page-with-a-single-introductory-section-B_2Wvxgi0). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the page depending on their device's screen size (from 320px up to 1920px).
- See hover and focus states for all interactive elements on the page.
- Experience a highly readable interface with a mathematically consistent typography system that respects browser zoom preferences.

### Screenshot

![Design Preview](/screenshot.jpg)

### Links

* Live URL: **[Huddle Landing Page](https://devkatiareis.github.io/FrontendMentor-huddle-landing-page-code-challenge/)**
* Solution URL: **[Frontend Mentor Solution](https://www.frontendmentor.io/solutions/responsive-landing-page-with-semantic-html-css-and-accessibility-NK1KFDCkCw)**
* Project Repo URL: **[GitHub Repository](https://github.com/devkatiareis/FrontendMentor-huddle-landing-page-code-challenge)**

## My process

### Built with

- Semantic **HTML5** markup (Landmarks: `<header>`, `<main>`, `<footer>`).
- **CSS Custom Properties** (Design Tokens).
- **Flexbox** for responsive layout control.
- **Mobile-first** workflow.
- **Modular Typography Scale** based on a **1.25 ratio (Major Third)**.
- **Accessibility** standards compliance (**WCAG 1.4.4**).

### What I learned

During this project, I focused on building a robust design system rather than just styling individual elements. One of the key takeaways was implementing a **Modular Scale** using the **1.25 ratio**, which ensures that the relationship between headings and body text is intentional and visually harmonious.

**Key technical highlights:**
- **Zoom Accessibility:** By using relative units (`rem`) and avoiding pure viewport units (`vw`) for font sizes, I ensured the layout remains compliant with **WCAG 1.4.4**, allowing the text to scale up to 200% without breaking the design.
- **Design Tokens:** I organized CSS variables into primitive and semantic tokens, allowing for easy mode-switching (Mobile/Desktop) and improved maintainability.
- **Readability (CPL):** I applied a "readability sweet spot" by limiting the paragraph containers to approximately **65 characters per line (65ch)** to reduce eye fatigue on larger screens.

**Responsive scale implementation example:**
```css
:root {
  /* Mobile base: 16px */
  --font-base: 1rem; 
  --text-4xl: 3.052rem; /* H1 mathematically scaled */
}

@media (min-width: 768px) {
  :root {
    /* Desktop base: 18px to account for reading distance */
    --font-base: 1.125rem; 
  }
}
```

### Continued development

In future projects, I intend to automate the handoff process using **Figma Variables** more extensively and dive deeper into **WAI-ARIA** patterns to improve accessibility for complex dynamic components.

### Useful resources

- [MDN Web Docs - Accessibility](https://developer.mozilla.org/en-US/docs/Web/Accessibility) - The primary reference for building inclusive web experiences.
- [Responsive Typography That Actually Works](https://medium.com) - This article was instrumental in understanding why `clamp()` can fail accessibility tests and how to use modular scales instead.
- [Google Fonts](https://fonts.google.com) - Used the **Poppins** (Headings) and **Open Sans** (Body) font families as specified in the style guide.

## Author

* Website - [Katia Reis](https://www.katiareis.com.br)
* Frontend Mentor - [@devkatiareis](https://www.frontendmentor.io/profile/devkatiareis)
* LinkedIn - [Katia Reis](https://www.linkedin.com/in/katiareis/)
