# Frontend Mentor - Testimonials grid section solution

This is a solution to the [Testimonials grid section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

![Frontend Mentor _ Testimonial grid section  - Google Chrome 07-04-2024 18_13_20](https://github.com/babybhavani/testimonialGrid/assets/152834101/2031663e-a063-411e-94a9-0240dac8a390)

### Links

- Solution URL: [Add solution URL here](https://github.com/babybhavani/testimonialGrid.git)
- Live Site URL: [Add live site URL here](https://babybhavani.github.io/testimonialGrid/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- [Styled Components](https://styled-components.com/) - For styles

### What I learned

I have learned about css grid and spanning the grid layout. Arranging and making the grid responsive for various view ports. Addition with, grabbed the knowledge and importance of usage of rem in website layouts.  

```html
<h1>Some HTML code I'm proud of</h1>
 <div class="card_1">
        <figure>
          <img src="images\image-daniel.jpg" alt="daniel-profile" class="card_1_img">
        </figure>
        <section class="card_1_user_data">
          <h1 class="user_name"> Daniel Clifford</h1>
          <h2 class="user_state"> Verified Graduate </h2>
        </section>
        <div class="card_1_testimony">
          <p class="header1">
            I received a job offer mid-course, and the subjects I learned were current, if not more so,
            in the company I joined. I honestly feel I got every penny’s worth.
          </p>
          <p class="footer1">
            “ I was an EMT for many years before I joined the bootcamp. I’ve been looking to make a
            transition and have heard some people who had an amazing experience here. I signed up
            for the free intro course and found it incredibly fun! I enrolled shortly thereafter.
            The next 12 weeks was the best - and most grueling - time of my life. Since completing
            the course, I’ve successfully switched careers, working as a Software Engineer at a VR startup. ”

          </p>
        </div>
      </div>
```
```css
.proud-of-this-css {
  color: papayawhip;
}

@media screen and (max-width: 1140px) {

    .subcontainer {
        width: 828px;
        height: 864px;
        grid-template-columns: repeat(3, 256px);
        grid-template-rows: 284px 266px 266px;
    }

    .card_2 {
        grid-column: 1 / 2;
        grid-row: 2 / 3;
        /* background-color: var(--very-dark-grayish-blue); */
    }

    .card_3 {
        grid-column: 2 / 3;
        grid-row: 2 / 3;
        background-color: var(--white);
    }

    .card_4 {
        grid-column: 1 / 3;
        grid-row: 3 / 4;
        /* background-color: var(--very-dark-blackish-blue); */
    }

    .card_5 {
        grid-column: 3 / 4;
        grid-row: 1 / 3;
        /* background-color: var(--white); */
    }

}

@media screen and (max-width: 860px) {

    body {
        align-items: flex-start;
    }

    .container {
        padding: 5rem 0;
    }

    .subcontainer {
        width: 542px;
        height: 1424px;
        grid-template-columns: repeat(2, 256px);
        grid-template-rows: 284px repeat(4, 266px);
    }

    .card_5 {
        grid-column: 1 / -1;
        grid-row: 4 / 5;
        /* background-color: var(--white); */
    }

}

@media screen and (max-width: 580px) {

    .subcontainer {
        height: auto;
        grid-template-columns: 328px;
        grid-template-rows: 444px 240px 222px 384px 438px;
        justify-content: center;
    }

    .card_1 {
        grid-column: auto;
        grid-row: 1 / 2;
        /* background-color: var(--moderate-violet); */
        background-position-x: 200px;
    }

    .header1 {
        letter-spacing: .011rem;
    }
    
    .footer1 {
        letter-spacing: .023rem;
    }

    .footer2 {
        font-size: .82rem;
        font-weight: 400;
        line-height: 1.13rem;
        letter-spacing: .007rem;
        opacity: .6;
    }

    .card_3 {
        grid-column: auto;
        grid-row: 3 / 4;
        /* background-color: var(--white); */
    }

    .card_4 {
        grid-column: auto;
        grid-row: 4 / 5;
        /* background-color: var(--very-dark-blackish-blue); */
    }

    .card_5 {
        grid-column: auto;
        grid-row: 5 / 6;
        /* background-color: var(--white); */
    }

    .footer5 {
        font-size: .83rem;
        font-weight: 400;
        line-height: 1.13rem;
        letter-spacing: .002rem;
        opacity: .7;
    }

}
```


### Continued development

I want to develop this upto adding more webpages to this section.

### Useful resources

- [CSS GRID](https://cssgrid.io/) - This helped me for XYZ reason. I really liked this pattern and will use it going forward.

## Author
- Frontend Mentor - [@babybhavani](https://www.frontendmentor.io/profile/yourusername)

