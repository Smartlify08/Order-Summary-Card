# Frontend Mentor - Order summary card solution

This is a solution to the [Order summary card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/order-summary-component-QlPmajDUj). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
- [Built with](#built-with)

  - [What I learned](#what-i-learned)

- [Author](#author)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- See hover states for interactive elements

### Screenshot

![](./screenshot/Order%20Summary%20Mobile.png)

![](./screenshot/Order-Summary%20Desktop.png)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow
- [Styled Components](https://styled-components.com/) - For styles

### What I learned

I learnt how to use before pseudo selector to do the plan text box section so the image background will be visible as it is the same background-color with the box

```html
<div class="text-box d-flex" role="textbox group">
  <div class="img-box">
    <img src="images/icon-music.svg" alt="" />
  </div>

  <div class="plan-text d-flex">
    <h3 class="text-dark">Annual Plan</h3>
    <h3 class="text-fade">$59.99/year</h3>
  </div>

  <div class="change-text">
    <a href="#" class="text-primary">Change</a>
  </div>
</div>
```

```css
.card-body .text-box {
  justify-content: space-between;
  align-items: center;
  padding: 10px 10px;
  border-radius: 6px;
  position: relative;
  z-index: 1;
}

.card-body .text-box::after {
  content: "";
  background-color: var(--clr-secondary);
  width: 100%;
  height: 100%;
  opacity: 50%;
  border-radius: 6px;
  z-index: -1;
  position: absolute;
  left: 0;
}
```

## Author

- Website - [Add your name here](https://smartlify08.github.io/Portfolio-Website/)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/Smartlify08)
- Twitter - [@yourusername](https://www.twitter.com/Smartlify)

**Note: Delete this note and add/remove/edit lines above based on what links you'd like to share.**
