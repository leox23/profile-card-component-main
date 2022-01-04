# Profile card component solution

This is a solution to the [Profile card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/profile-card-component-cfArpWshJ). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

- Build out the project to the designs provided

### Screenshot

![1](./images/chrome_0t8uC0BriF.png)

### Links

- Solution URL: [Github repositorie](https://github.com/leox23/profile_card_component)
- Live Site URL: [Live site](https://leox23.github.io/profile_card_component/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flex-box
- CSS Grid
- Mobile-first workflow

### What I learned

There are things that I could solve on the road and that they were necessary to replicate the challenge as the same as possible:

I had problems to fully stretch the background of the user image, for no method from CSS I could, so I knew and change the width of the SVG from the file itself, which can be done directly from CSS if the correct properties are used:
```html
<svg width="978" height="978" xmlns="http://www.w3.org/2000/svg">...
```

In the HTML you can use a special "invisible" character in order to add more separation space to a word specifically, instead of using the CSS letter-spacing as in the example of the image:
```html
      ↓
<span>⠀26</span>
```
![1](./images/chrome_xULZ4Cm5cB.png) 

In CSS for properties with several blocks of values ​​that are separated by comma, you can place one below one for better readability:
```css
body{
    ...
    background: url(images/bg-pattern-top.svg) -740px -640px no-repeat,
                url(images/bg-pattern-bottom.svg) 118px 270px no-repeat,
                #19A1AD;
}
```

Using the CSS BEM methodology, we have to be careful with the name of the classes, it will make elements that interfere with class names do not show correctly:

```Css
.child-container {
    ... some rules ...
}
/*=========================*/
.social-container { 🚫❌❌❌
    🚫The Container class is repeated, an
    unnoticed error, and is not showed correctly.
}

.social {✅
    ✅ Better solution
}

```

### Continued development

Specifically, my future goal for the kind of skills in this challenge, is to be able to use Flex-box and CSS Grid in larger and more complex page layouts, and to be faster at debugging CSS in general, **just because it's not a programming language, doesn't mean it's not complex.**

### Useful resources

- [W3Schools](https://www.w3schools.com/) - Excellent tool for fast CSS queries in case of doubts.
- [Css Tricks](https://css-tricks.com/) - This specific site I like to support me in the complete articles of [Flex-Box](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) and [Grid](https://css-tricks.com/snippets/css/complete-guide-grid/#prop-grid).
- [ShareX](https://getsharex.com/) - Great software that I use in my day by day, in this case, use the rule, the color picker and the magnifying glass.

## Author

- Github - [leox23](https://github.com/leox23)
- Frontend Mentor - [@leox23](https://www.frontendmentor.io/profile/leox23)


