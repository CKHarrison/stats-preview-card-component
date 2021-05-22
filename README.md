# Frontend Mentor - Stats preview card component solution

This is a solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Frontend Mentor - Stats preview card component solution](#frontend-mentor---stats-preview-card-component-solution)
  - [Table of contents](#table-of-contents)
  - [Overview](#overview)
    - [The challenge](#the-challenge)
    - [Screenshot](#screenshot)
    - [Links](#links)
  - [My process](#my-process)
    - [Built with](#built-with)
    - [What I learned](#what-i-learned)
    - [Useful resources](#useful-resources)
  - [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size

### Screenshot

![Mobile View](/screenshots/mobile-screenshot.png)
![Desktop View](/screenshots/desktop-screenshot.png)

### Links

- Solution URL: [Solution URL](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62/hub/stats-preview-card-component-zs7x4zJoO)
- Live Site URL: [Live Site Demo](https://ckharrison.github.io/stats-preview-card-component/)

## My process
I used this challenge to help solidify my knowledge of responsive design using CSS Grid and Flexbox. I started out creating the mobile design first and then went ahead and implemented the desktop design via a media query.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

The most challenging part about this design was adding a tint/colored overlay to the hero image. This is the first time I have done something like this via CSS. Normally I would have just added in the tint via photoshop, but I decided to take the time to learn how to do this via CSS only. 
I was able to accomplish this by adding in a div container over the hero image, and using the wrapping div's :after pseudo property to add in the overlay tint.

```
.hero::after {
  content: '';
  display: block;
  position: absolute;
  height: 100%;
  width: 100%;
  background: var(--violet-accent-image);
  opacity: .5;
  top: 0;
  left: 0;
  
}

```

I also learned how to add responsive images depending on the viewport's screensize using the srcset image attribute. I've never done that before so this was a fun new thing to learn.

### Useful resources

- [Ideabase - Adding Image overlay tint](https://ideabasekent.com/wiki/adding-image-overlay-tint-using-css) - I was able to use this article as a resource on how to tint an image. I found it incredibly helpful.
- [CSS Tips and Tricks - Guide to Responsive Images](https://css-tricks.com/a-guide-to-the-responsive-images-syntax-in-html/#using-srcset) - This was a useful article that helped me with responsive images.

## Author

- Website - [CKHarrison](https://github.com/CKHarrison)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/ckharrison)