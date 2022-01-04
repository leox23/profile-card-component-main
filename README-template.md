# Frontend Mentor - Profile card component solution

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
- [Acknowledgments](#acknowledgments)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

- Build out the project to the designs provided

### Screenshot

![](./screenshot.jpg)

Add a screenshot of your solution. The easiest way to do this is to use Firefox to view your project, right-click the page and select "Take a Screenshot". You can choose either a full-height screenshot or a cropped one based on how long the page is. If it's very long, it might be best to crop it.

Alternatively, you can use a tool like [FireShot](https://getfireshot.com/) to take the screenshot. FireShot has a free option, so you don't need to purchase it. 

Then crop/optimize/edit your image however you like, add it to your project, and update the file path in the image above.

**Note: Delete this note and the paragraphs above when you add your screenshot. If you prefer not to add a screenshot, feel free to remove this entire section.**

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- [React](https://reactjs.org/) - JS library
- [Next.js](https://nextjs.org/) - React framework
- [Styled Components](https://styled-components.com/) - For styles

**Note: These are just examples. Delete this note and replace the list above with your own choices**

### What I learned

Use this section to recap over some of your major learnings while working through this project. Writing these out and providing code samples of areas you want to highlight is a great way to reinforce your own knowledge.

To see how you can add code snippets, see below:

I had problems to fully stretch the background of the user image, for no method from CSS I could, so I knew and change the width of the SVG from the file itself, which can be done directly from CSS if the correct properties are used:
```html
<svg width="978" height="978" xmlns="http://www.w3.org/2000/svg">...
```

In the HTML you can use a special "invisible" character in order to add more space to a word specifically, instead of using the CSS letter-spacing as in the example of the image:
```html
	  ↓
<span>⠀26</span>
```
![1](.\images\chrome_xULZ4Cm5cB.png)

In CSS for properties with several blocks of values ​​that are separated by comma, you can place one below one for better readability:
```css
body{
    ...
    background: url(images/bg-pattern-top.svg) -740px -640px no-repeat,
                url(images/bg-pattern-bottom.svg) 118px 270px no-repeat,
                #19A1AD;
}
```

Using the CSS BEM methodology, you have to be careful with the name of the classes, it will make elements that interfere with class names do not show correctly:

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

Use this section to outline areas that you want to continue focusing on in future projects. These could be concepts you're still not completely comfortable with or techniques you found useful that you want to refine and perfect.

**Note: Delete this note and the content within this section and replace with your own plans for continued development.**

### Useful resources

- [W3Schools](https://www.w3schools.com/) - Excellent tool for fast CSS queries in case of doubts.
- [Css Tricks](https://css-tricks.com/) - This specific site I like to support me in the complete articles of [Flex-Box](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) and [Grid](https://css-tricks.com/snippets/css/complete-guide-grid/#prop-grid).
- [ShareX](https://getsharex.com/) - Great software that I use in my day by day, in this case, use the rule, the color picker and the magnifying glass.

**Note: Delete this note and replace the list above with resources that helped you during the challenge. These could come in handy for anyone viewing your solution or for yourself when you look back on this project in the future.**

## Author

- Website - [Add your name here](https://www.your-site.com)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)
- Twitter - [@yourusername](https://www.twitter.com/yourusername)

**Note: Delete this note and add/remove/edit lines above based on what links you'd like to share.**

## Acknowledgments

This is where you can give a hat tip to anyone who helped you out on this project. Perhaps you worked in a team or got some inspiration from someone else's solution. This is the perfect place to give them some credit.

**Note: Delete this note and edit this section's content as necessary. If you completed this challenge by yourself, feel free to delete this section entirely.**
