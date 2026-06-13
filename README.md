# Razorpay Clone 🚀

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)

A responsive, pixel-perfect frontend clone of the **Razorpay** landing page. Built purely using semantic HTML5, Vanilla CSS3, and standard JavaScript. This project replicates Razorpay's modern, beautiful, and dynamic landing page layout, showcasing advanced UI/UX components.

---

## 🎨 Visual Preview

![Razorpay Clone Banner](./razorpay_clone_banner.png)

*A modern design showcasing Razorpay's iconic aesthetic, payment gateway features, and global payment dashboard UI.*

---

## 📌 Table of Contents

1. [Features](#-features)
2. [Technologies Used](#-technologies-used)
3. [Project Structure](#-project-structure)
4. [Getting Started](#-getting-started)
5. [Technical Implementation Details](#-technical-implementation-details)
   - [CSS Grid & Flexbox](#1-css-grid--flexbox)
   - [Infinite Marquee Animation](#2-infinite-marquee-animation)
   - [Mobile Responsiveness](#3-mobile-responsiveness)
6. [Minor Enhancements & Fixes](#-minor-enhancements--fixes)
7. [License](#-license)

---

## ✨ Features

- **Pixel-Perfect Hero Section**: Modern typography, clean layout, CTA buttons, and a responsive structure.
- **Infinite Logo Marquee**: An animated brand ticker/slider displaying partner companies (Ola, Zomato, Blinkit, Swiggy, etc.) with smooth infinite horizontal scrolling.
- **Product Suite Showcase**: Features grid displays for Razorpay's payment gateway, subscription billing, smart collect, route, banking suite, and developer tools.
- **Interactive Action Buttons**: Visual feedback on hover and active states. Includes JavaScript modal triggers for demo states.
- **100% Responsive Design**: Styled from scratch to look stunning on mobile, tablet, and desktop viewports using CSS Media Queries.
- **Clean Structure**: Highly semantic and well-commented HTML elements.

---

## 🛠️ Technologies Used

- **HTML5**: Used semantic markup (`<header>`, `<nav>`, `<section>`, `<footer>`) to construct the layout and improve SEO searchability.
- **Vanilla CSS3**: Styled using advanced layout properties, gradients, grid items, flex container distributions, and keyframe animations.
- **JavaScript (ES6+)**: Handles basic click events and user interactions (e.g., warning notifications for demo mode limits).
- **SVG Vector Graphics**: Embedded for high-resolution graphics that scale seamlessly on all screen sizes.

---

## 📂 Project Structure

```text
Razorpay-Clone/
├── global-payments.svg       # SVG Illustration for Currencies/Banking section
├── hero.svg                  # SVG Illustration for the Hero section
├── razorpay_clone_banner.png # Generated project banner/screenshot
├── index.html                # Main HTML & CSS project file (previously razorpayclone.html)
└── README.md                 # Documentation file
```

---

## 🚀 Getting Started

To view the landing page clone locally on your system:

### Option 1: Direct File Open
1. Double-click the `index.html` file in your file explorer.
2. It will open directly in your preferred web browser.

### Option 2: Live Server (Recommended)
If using VS Code:
1. Open the repository folder in VS Code.
2. Install the **Live Server** extension.
3. Click **Go Live** at the bottom-right corner to run the application on a local development server.

---

## ⚙️ Technical Implementation Details

### 1. CSS Grid & Flexbox
The sections are built using **CSS Grid** and **CSS Flexbox** to construct modern card displays and layouts:
```css
.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 30px;
}
```
This ensures that cards adjust automatically in density depending on the available viewport width.

### 2. Infinite Marquee Animation
An elegant infinite sliding animation is achieved via pure CSS keyframes:
```css
.brand-track {
  display: flex;
  width: fit-content;
  animation: marquee 24s linear infinite;
}

@keyframes marquee {
  from { transform: translateX(0); }
  to { transform: translateX(-50%); }
}
```

### 3. Mobile Responsiveness
Media queries are used to convert grid sections into vertical list stacks on mobile screens:
```css
@media(max-width: 900px) {
  .hero { grid-template-columns: 1fr; }
  .global { grid-template-columns: 1fr; }
}
```

---

## 🛠️ Minor Enhancements & Fixes
- **Corrected HTML Syntax**: Closed the `brand-track`, `brand-slider`, and `brands` section wrappers to prevent layout bleeding into subsequent sections.
- **Clean Code formatting**: Cleaned up the tag hierarchy to ensure all elements are valid under standard HTML validation protocols.

---

## 📄 License

This project is licensed under the MIT License. Feel free to use and modify it for your own learning and development purposes.
