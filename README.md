# Frontend Mentor - Testimonials grid section solution

This is a solution to the
[Testimonials grid section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7).
Frontend Mentor challenges help you improve your coding skills by building
realistic projects.

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
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Screenshot

![iPhone] (./screenshots/iPhone-12-PRO-127.0.0.1%20(1).png) ![Macbook]
(./screenshots/Macbook-Air-127.0.0.1%20(4).png)

### Links

- Solution URL:
  (https://github.com/Mubarak-Adeyemi/testimonials-grid-section-main)
- Live Site URL:
  (https://mubarak-adeyemi.github.io/testimonials-grid-section-main/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

I used semantic tags like <section>, <figure>, <figcaption>, and <blockquote> to
organize and present testimonials. This enhances both readability and
accessibility.

The layout is responsive, thanks to CSS Grid. I defined different grid templates
for mobile (grid-template-columns: 1fr;) and larger screens using media queries
(grid-template-columns: 1fr 1fr 1fr 1fr;).

I used the ::after pseudo-element to display a background quotation pattern on
one of the testimonial cards.

```html
<section class="testimonials">
  <div class="testimonial-card card-1">
    <figure class="testimonial">
      <figcaption>
        <img src="./images/image-daniel.jpg" alt="Photo of Daniel Clifford" />
        <h2>Daniel Clifford</h2>
        <p class="descr">Verified Graduate</p>
      </figcaption>
      <blockquote>
        <p class="lead-p">I received a job offer mid-course...</p>
        <p class="sub-p">
          “I was an EMT for many years before I joined the bootcamp...”
        </p>
      </blockquote>
    </figure>
  </div>
</section>
```

```css
.testimonials {
  display: grid;
  grid-template-columns: 1fr;
  gap: 2rem;
}
.testimonial-card {
  padding: 2rem;
  border-radius: 8px;
  background-color: var(--Moderate-violet);
}
img {
  width: 2.5rem;
  border-radius: 50%;
}

@media (min-width: 768px) {
  .testimonials {
    grid-template-columns: 1fr 1fr 1fr 1fr;
    grid-template-areas:
      "card1 card1 card2 card5"
      "card3 card4 card4 card5";
  }
}
```

### Continued development

I'll try adding a carousel for testimonials to help make the page more
interactive and less cluttered on smaller screens.

I'll also try adding testimonials dynamically with javascript.

### Useful resource

- [CSS Tricks](https://css-tricks.com/snippets/css/complete-guide-grid/) - This
  is an amazing article which helped me understand CSS grid better. I'd
  recommend it to anyone still learning this concept.

## Author

- Frontend Mentor -
  [@Mubarak-Adeyemi](https://www.frontendmentor.io/profile/Mubarak-Adeyemi)
- Twitter - [@mubarakElarabiy](https://www.twitter.com/mubarakElarabiy)

## Acknowledgments

Thanks to frontend mentor!
