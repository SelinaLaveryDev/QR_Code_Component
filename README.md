# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://selinalaverydev.github.io/QR_Code_Component/). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)

## Overview

### The Brief

Your challenge is to build out this QR code component and get it looking as close to the design as possible.

You can use any tools you like to help you complete the challenge. So if you've got something you'd like to practice, feel free to give it a go.

Download the starter code and go through the README.md file. This will provide further details about the project. The style-guide.md file is where you'll find colors, fonts, etc.

### Screenshot

![QR Code Component](https://sel-dev-bucket.s3.us-east-1.amazonaws.com/Frontend-mentor/Screenshot+2025-02-23+at+18.27.36.png)

## Links
View my solution [here](https://selinalaverydev.github.io/QR_Code_Component/)

## My process

- Revised the instructions and design documents
- Defined CSS variables for text presets set out in the figma file
- Wrote up semantic HTML
- Used flexbox for responsiveness

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

I learned how quickly Figma can help define CSS variables for text presets.
```css
:root {
  /* colours */
  --slate-900: #1f314f;
  --slate-500: #68778d;
  --slate-300: #d5e1ef;
  --blue-600: #2c7dfa;
  --blue-500: #3685ff;
  --blue-400: #4d9ffc;
  --white-100: #ffffff;

  /* typography */
  --font-outfit-bold: Outfit, sans-serif;
  --font-outfit-regular: Outfit, sans-serif;

  --text-outfit-bold-size: 22px;
  --text-outfit-bold-line-height: 120%;
  --text-outfit-bold-spacing: 0px;

  --text-outfit-regular-size: 15px;
  --text-outfit-regular-line-height: 140%;
  --text-outfit-regular-spacing: 0.2px;
}
```
Created classes using the variables to match with the Figma design styles
```classes
.outfit-bold {
  font-family: var(--font-outfit-bold);
  font-size: var(--text-outfit-bold-size);
  line-height: var(--text-outfit-bold-line-height);
  letter-spacing: var(--text-outfit-bold-spacing);
  color: var(--slate-900);
  text-align: center;
  margin-bottom: 16px;
}

.outfit-regular {
  font-family: var(--font-outfit-regular);
  font-size: var(--text-outfit-regular-size);
  line-height: var(--text-outfit-regular-line-height);
  letter-spacing: var(--text-outfit-regular-spacing);
  color: var(--slate-500);
  text-align: center;
}

```
Here, I used semantic HTML where I could for SEO
```semantic HTML
      <section class="container">
```
Initially I used a 'p' element, but realised that using an 'h1' helped match the brief more accurately
```semantic HTML
      <h1 class="outfit-bold">
          Improve your front-end skills by building projects
      </h1>
```
Used 'alt' attribute for accessibility and 'lazy loading' for the image to prevent slo page loading
```accessibility
        <img
          src="./images/image-qr-code.png"
          alt="QR code"
          class="qr-code"
          loading="lazy"
        />
```

## Author

- [My Portfolio Website](https://selinalaverydev.github.io/selina-dev-portfolio/)
- [My Frontend Mentor Profile](https://www.frontendmentor.io/profile/SelinaLaveryDev)
- [My Github Profile](https://github.com/SelinaLaveryDev)
