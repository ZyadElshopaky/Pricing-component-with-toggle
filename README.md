# 💰 Frontend Mentor - Pricing Component with Toggle Solution

This is a solution to the [Pricing Component with Toggle challenge](https://www.frontendmentor.io/challenges/pricing-component-with-toggle-8vPwRMIC) on Frontend Mentor.  
Frontend Mentor challenges help you improve your coding skills by building realistic projects.

---

## 📋 Table of Contents
- [Overview](#overview)
- [The Challenge](#the-challenge)
- [Screenshot](#screenshot)
- [Links](#links)
- [My Process](#my-process)
  - [Built With](#built-with)
  - [What I Learned](#what-i-learned)
  - [Continued Development](#continued-development)
  - [Useful Resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

---

## 🧩 Overview

### The Challenge
Users should be able to:
- View the optimal layout for the component depending on their device's screen size  
- Toggle between **monthly** and **annual** pricing  
- Control the toggle with both their mouse/trackpad and their keyboard  
- **Bonus**: Complete the challenge using only HTML and CSS  

---

### 🖼️ Screenshot

![Pricing Component Screenshot](./design/desktop-preview.jpg)

---

### 🔗 Links
- **Solution URL:** [Frontend Mentor Solution](https://www.frontendmentor.io/solutions/)
- **Live Site URL:** [Live Demo](https://your-live-site-url.com)

---

## 🧠 My Process

### ⚙️ Built With
- Semantic **HTML5 markup**  
- **CSS custom properties**  
- **Flexbox** & **CSS Grid**  
- **Vanilla JavaScript** for toggle functionality  
- **Mobile-first workflow**

---

### 💡 What I Learned
While working on this challenge, I learned how to:
- Use CSS variables and gradients for consistent theming  
- Implement a toggle switch using only HTML, CSS, and JavaScript  
- Build a fully responsive pricing layout  
- Manage visibility dynamically using JavaScript classes  

Example of the toggle logic I used:
```js
const toggle = document.getElementById('toggle');
const annualPrices = document.querySelectorAll('.annual');
const monthlyPrices = document.querySelectorAll('.monthly');

toggle.addEventListener('change', () => {
  const showMonthly = toggle.checked;
  annualPrices.forEach(p => p.classList.toggle('hidden', showMonthly));
  monthlyPrices.forEach(p => p.classList.toggle('hidden', !showMonthly));
});
```

---

### 🚀 Continued Development
In the future, I’d like to:
- Add animations when switching between pricing modes  
- Improve accessibility using ARIA attributes  
- Explore creating the same project using React or Svelte  

---

### 📚 Useful Resources
- [MDN Web Docs](https://developer.mozilla.org/en-US/) – For quick HTML/CSS/JS reference  
- [Frontend Mentor Community](https://www.frontendmentor.io/community) – Helpful discussions and examples  

---

## 👨‍💻 Author

- **Name:** Zyad Elshopaky  
- **Frontend Mentor:** [@ZyadElshopaky](https://www.frontendmentor.io/profile/ZyadElshopaky)  
- **GitHub:** [ZyadElshopaky](https://github.com/ZyadElshopaky)  

---

## 🙌 Acknowledgments
Thanks to **Frontend Mentor** for providing this amazing challenge.  
It was a great opportunity to practice responsive design and clean UI implementation.
