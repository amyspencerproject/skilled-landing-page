# Frontend Mentor - Skilled e-learning landing page solution

This is a solution to the [Skilled e-learning landing page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/skilled-elearning-landing-page-S1ObDrZ8q). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)


## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

### Built with

- HTML5 
- CSS custom properties
- Flexbox
- Mobile-first workflow


### What I learned

I have only used pseudo elements once before this project. Typing "pseudo" alone into a search is not spefic enough. I needed to use pseudo elements specifically and it took me a little bit to realize this. I needed a ::before to get course icons to sit just halfway above the top of the card.
[MDN on ::before](https://developer.mozilla.org/en-US/docs/Web/CSS/::before)

Used the ```<picture>``` element to make the hero image responsive. This challenge has the image spilling off the page for tablet screen sizes and larger. I stuggled to get this accomplished. Was not sure what the best practice should be to get this effect. I can do this quickly by putting a height of 500px on the image container. Instead I tried to use transform: translateX(), position: absolute, and postion: relative in combination with object-fit: and overflow:. Initially submitted this challenge knowing that I had not optimized the hero image.

Discovered that the order of the ```<source>``` elements matter inside the ```<picture>```. The following code was not working when the 768px query was listed before the 1200px query.
```
  <picture class="hero-image">
    <source media="(min-width: 1200px)" srcset="./assets/image-hero-desktop.png" />
    <source media="(min-width: 768px)" srcset="./assets/image-hero-tablet.png" />
    <img class="product-image" src="./assets/image-hero-mobile.png" 
          alt="Femastudent sipping coffee" />
  </picture>
```

Feedback from Frontend Mentro - use absolute positioning on the imgage and relative on the container holding the image. This worked! I positioned the image in the container div that holds the image with absolute. Then I positioned the container div with position relative. I added a bottom margin on the hero section of 14rem to keep rest of the content from sliding under the hero image.

Another aspect of this challenge I wasn't sure hot to solve was positioning all the Get Started links. Each link needs to sit at the bottomo of the card but height of the content in the cards are different. The advice from Frontend Mentor was to use flex column and then margin top auto to push the links to the bottom of the cards. I did this plus put a min-height on the paragrah of 9.4rem and set align-items:stretch.


### Continued development

Still not fully understanding the use of position, object-fit, and overflow. Especially with making a seemless responsive site. Stipulating the height is a the easy way out and I am trying hard to develop the skills to not do this.

## Author

- Website - [Amy Spencer](https://spencerproject.com/)
- Frontend Mentor - [@amyspencerproject](https://www.frontendmentor.io/profile/amyspencerproject)
- Linkedin - [amyspencercodes](https://www.linkedin.com/in/amyspencercodes/)