# Frontend Mentor - Stats preview card component solution

This is a solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)


## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size

### Screenshot

![Desktop View](./design/desk_des.jpg)

![Mobile View](./design/mobile_des.jpg)


### Links

- Solution URL: [My Solution](https://www.frontendmentor.io/solutions/stats-preview-card-solution-WBZApsY6Eb)
- Live Site URL: [With GitHub](https://clipzorama.github.io/Stats-Preview-Card----F.M/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-Queries
- CSS `mix-blend-mode` for color overlays


### What I learned

- Color Blending Techniques: I explored and applied the `mix-blend-mode` property to overlay colors on top of images, which was new for me. This allowed me to add a subtle color effect to an image without changing the source file itself, giving the image a dynamic and stylish look. Definitely want to look more into this.

- Flexbox Layout: I solidified my understanding of Flexbox, especially when dealing with responsive designs that require different layouts on mobile and desktop devices. I learned how to change the order of elements without modifying the HTML using the order property in Flexbox. 



```html
<section class="all-content">
        <div class="card">
            <img class="top" src="./assets/images/illustration-article.svg" alt="Cool Picture here">
            <div class="label">Learning</div>
            <h5>Published 21 Dec 2023</h5>
            <h2>HTML & CSS foundations</h2>
            <p class="details">These languages are the backbone of every website, defining structure, content, and
                presentation.</p>
            <div class="signature">
                <img src="./assets/images/image-avatar.webp" alt="Greg" class="face">
                <p class="name">Greg Hooper</p>
            </div>
        </div>
    </section>
```

```css
.image-container::after {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: var(--Soft-violet);
    mix-blend-mode: multiply;
    opacity: 1;
}
```

### Continued development

In future projects, It would be cool to explore:

- CSS Variables & Theming: In this project, I made use of CSS custom properties for colors. I’d like to explore building more complex theming systems that could allow for easy design adjustments, such as light/dark themes. I've seen a couple videos on making this happen but haven't got into it yet.

- Animations: Adding smooth animations for element transitions, maybe like hovering over the stats or image, could enhance user experience. Thus, CSS keyframes and transitions will help me improve the interaction design of future projects.

## Author

- Frontend Mentor - [@Clipzorama](https://www.frontendmentor.io/profile/Clipzorama)

