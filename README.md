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


### Continued development

Use this section to outline areas that you want to continue focusing on in future projects. These could be concepts you're still not completely comfortable with or techniques you found useful that you want to refine and perfect.

## Author

- Website - [Amy Spencer](https://spencerproject.com/)
- Frontend Mentor - [@amyspencerproject](https://www.frontendmentor.io/profile/amyspencerproject)
- Linkedin - [amyspencercodes](https://www.linkedin.com/in/amyspencercodes/)