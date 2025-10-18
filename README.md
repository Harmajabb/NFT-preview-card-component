# Frontend Mentor - NFT Preview Card Component Solution

This is my first Frontend Mentor challenge: [NFT Preview Card Component](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U).  
It helped me get comfortable with **HTML structure**, **CSS variables**, **hover effects**, and **flexbox layout basics**.

---

## 🗂️ Table of Contents
- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My Process](#my-process)
  - [Built With](#built-with)
  - [What I Learned](#what-i-learned)
  - [Challenges & Solutions](#challenges--solutions)
  - [Future Improvements](#future-improvements)
- [Author](#author)

---

## 🪞 Overview

### The Challenge
Users should be able to:
- See hover states for interactive elements.
- View the card layout correctly on different screen sizes.
- See a hover overlay on the main NFT image.
- Understand the structure and spacing of elements using semantic HTML and CSS variables.


### Links
- 🌍 Live Site URL: [Add your live site link here](https://your-live-site-url.com)
- 📦 Repository: [https://github.com/Harmajabb/nft-preview-card](https://github.com/Harmajabb/nft-preview-card)

---

## My Process

### Built With
- Semantic **HTML5**
- **CSS custom properties** (`:root` variables)
- **Flexbox** for layout and alignment
- **Hover transitions** and pseudo-elements (`::before`, `::after`)
- **Mobile-first** approach
- File organization with `img/` and `styles/` folders

---

###  What I Learned
This was my first Frontend Mentor project, so I focused on mastering the fundamentals:
- How to use **CSS variables** for colors, fonts, and spacing.
- Building a clean **card layout** with consistent margins and paddings.
- Creating a **hover overlay effect** on an image using:
  ```css
  figure::before {
    content: "";
    position: absolute;
    inset: 0;
    background-color: var(--cyan);
    opacity: 0;
    transition: opacity 0.3s ease;
  }
  figure:hover::before {
    opacity: 1;
  }

### Challenges & Solutions
## Overlay and icon visibility on hover
- **Challenge:** Getting the hover overlay to appear smoothly over the NFT image.  
  **Solution:** I learned how to use `position: relative` on the `<figure>` and `position: absolute` on the pseudo-elements `::before` and `::after` to layer and center them properly.

## Vertical alignment with flexbox
- **Challenge:** The ETH price and time remaining wouldn’t align correctly on the same line.  
  **Solution:** I used `display: flex; justify-content: space-between; align-items: center;` to align icons and text evenly.

## Card centering on the page
- **Challenge:** At first, the card wasn’t centered on all screen sizes.
  **Solution:** I set the body as a flex container with `height: 100vh; display: flex; justify-content: center; align-items: center;` to perfectly center the component both vertically and horizontally.

### Future Improvements
- Add **responsive design** tweaks for smaller screens.
- Improve **accessibility** by adding proper alt text and link roles.
- Add **smooth transitions** for image hover and text color changes.

### Author 
- Lea Francois, student at Wild Code School, fullstack web development program.