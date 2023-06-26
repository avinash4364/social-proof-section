# Frontend Mentor - Social proof section solution

This is a solution to the [Social proof section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/social-proof-section-6e0qTv_bA).

## Table of contents

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

- View the optimal layout for the section depending on their device's screen size

### Screenshot

![127 0 0 1_5500_ (2)](https://github.com/avinash4364/social-proof-section/assets/24203618/285d8a5e-d356-45bb-baea-787a27ce62b6)
![127 0 0 1_5500_ (1)](https://github.com/avinash4364/social-proof-section/assets/24203618/bb4bf70f-07d0-4fe8-8703-1b9458713980)

### Links

- Solution URL: [solution URL](https://github.com/avinash4364/social-proof-section)
- Live Site URL: [live site URL](https://avinash4364.github.io/social-proof-section/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

- I learned about CSS `min()` and `max()` function and how it can be used to set a width of a container dynamically. In the below example basically we are setting the width of the container to maximum out of 2 values, which are `30rem` and `50%` the width of the parent container.

- So, here the container size will increase as soon as the width of the parent container increases beyond `2 * 30rem` (600px in our case) and it will be set to the `50%` of the parent container width.

```css
.container {
  width: max(30rem, 50%);
}
```

- For centering the whole content on the body both horizontally and vertically, we should always create a container(wrapper) around all the child elements of the body. It is not recommended to use `display:flex` on the body and center the container. As it will not be benificial in case of setting the background-image of the body absolutely. Instead, we can center the child elements by applying `display:flex` to the container or `margin:auto` (for horizontal alignment). We can give the background-image to the container which is absolutely positioned and this will not cause an overflow.

### Useful resources

- [freeCodeCamp article](https://www.freecodecamp.org/news/html-page-width-height/) - This helped me understand how to set height and width on the body and html tag in the CSS styling. Basically we set `min-height:100vh` on the body so the body can further expand beyond the viewport height if the content demands thus not causing an overflow if explicit height is specified. This also helps in setting body as a flex container and centering the content (but for that we should use a container).

## Author

- Frontend Mentor - [@avinash4364](https://www.frontendmentor.io/profile/avinash4364)
