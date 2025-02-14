# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![Screenshot of the NFT preview card component](./screenshot.gif)

### Links

- Solution URL: [Github](https://github.com/snigdha-sukun/nft-preview-card)
- Live Site URL: [Vercel](https://nft-preview-card-bay-ten.vercel.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- BEM
- CUBE CSS

### What I learned

I learned BEM naming conventions as well as how to structure my stylesheet using CUBE CSS method.

I learned how to center an object within the parent boundaries by using `place-items` and `display: grid` with `height` set to a value.

```css
body {
    display: grid;
    min-height: 100vh;
    place-items: center;
}
```

I learned how to create coloured image overlay

```css
.image__overlay {
    background-color: var(--cyan-light);
    display: none;
    width: auto;
    height: 100%;
    place-items: center;
    bottom: 100%;
    margin-bottom: 100%;
    position: relative;
}

.card__image:hover div.image__overlay{
    display: grid;
}
```

I learned how to add exceptions using CUBE method:

```css
.card__stats__value[data-type="ethereum"] {
    color: var(--cyan);
    font-weight: var(--font-weight-600);
}
```

### Continued development

I want to continue learning & practice different CSS methodologies.

### Useful resources

- [CUBE CSS methodology in action](https://www.youtube.com/watch?v=NanhQvnvbR8) - This video helped me in understanding how to go about using CUBE CSS in my code.
- [Show Colored Overlay on Image Hover using CSS](https://wisdmlabs.com/blog/show-color-overlay-image-hover-using-css/) - This helped me in creating coloured overlay on image when hovering as needed in the design.

## Author

- Frontend Mentor - [@snigdha-sukun](https://www.frontendmentor.io/profile/snigdha-sukun)
