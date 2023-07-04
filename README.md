# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)



## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Screenshot

![](./Desktop%20view.png)


### Links

- Solution URL: [Add solution URL here](https://github.com/MHA2001/product_preview_card)
- Live Site URL: [Add live site URL here](https://mha2001.github.io/product_preview_card/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- CSS variable
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

1. it is better to look at desktop design rather than mobile design when writing html (for css start with mobile)
2. an article is can be use whenever somthing could be sort of a standalone piece of content.

```html
<picture class="product__image">
  <source srcset="./images/image-product-desktop.jpg" media="(min-width: 600px)">
  <img src="./images/image-product-mobile.jpg" alt="" />
</picture>
<!--  -->
<button class="button" data-icon="shopping-cart">Add to Cart</button>
```
```css
.button:is(:hover, :focus){
    background-color: var(--clr-primary-500);
}
.button[data-icon="shopping-cart"]::before{
    content: "";
    width: 15px;
    height: 16px;
    background-image: url(./images/icon-cart.svg);

}
```



