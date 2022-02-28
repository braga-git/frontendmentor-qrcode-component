# Frontend Mentor - QR code component solution

Wassup! :call_me_hand:	

This is my solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). 

Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
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

### Screenshot

![My solution](https://github.com/braga-git/frontendmentor-qrcode-component/blob/main/design/mydesktop-design.png)

### Links

- [Solution codes](https://github.com/braga-git/frontendmentor-qrcode-component)
- [Live site](https://braga-git.github.io/frontendmentor-qrcode-component/)

## My process

### Built with

- HTML5
- CSS3

### What I learned

As I'm too young in this world and just started to learn HTML and CSS, the hardest for me to do alone was to actually know where to start. :sweat_smile:	

From my point of view, this challenge is more a CSS challenge than a HTML5 one. My biggest difficulties were about alignment and the interaction between `<img>` and `<div>`, as sometimes I was trying to configurate the div's padding and the img popped out of the div. 

This was very easy to fix, I simply used the `overflow` property with the `hidden` value:

```css
div.window-qr {
  overflow: hidden;
} 
```

This code hiddes the content that exceeds the div. 

I fixed the issue of the img getting off the div, but it still wasn't centered. It kept a left margin and was displaying higher than I wanted. To fix it I setted the `img width` to `100%`.

```css
.window-qr img {
        width: 100%;
}
```

This made the image occupy only the width of the div.

The last problem I had to solve was how to center my content either horizontally and vertically. This one I really didn't know how to do, but I searched and did found a way that worked. I used the property `transform` with `translate` value:

```css
main {
    position: fixed;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}
```

And I don't really know how this code works, but..

In sum, I think I handled it really good. Well, even if the code isn't the best, the design is pretty close! :rofl:		

### Continued development

I'll keep looking for ways to center things properly because, as I said, I don't know 100% the usability and function of the `transform` property. **But I do know that it's not ok to use a code without knowing how it works**. :man_shrugging:	

### Useful resources

- [Alignment code source](https://css-tricks.com/quick-css-trick-how-to-center-an-object-exactly-in-the-center/) - This is where I found the alignment code with the `transform` property. The funny thing is that it was posted almost 15 years ago.
- [Transform property explanation](https://developer.mozilla.org/en-US/docs/Web/CSS/transform) - This gives you an explanation about the property functions.

## Author

Follow me for more "solutions" :wink: 

- Frontend Mentor - [@braga-git](https://www.frontendmentor.io/profile/braga-git)
- Instagram - [@braga.jpeg](https://www.instagram.com/braga.jpeg/)
- LinkedIn - [Gabriel Braga Camara](https://www.linkedin.com/in/gabrielbragacamara/)

## Acknowledgments

Thanks to [@chriscoyier](https://github.com/chriscoyier) for the post about the `transform` function. I was 6 by that time! :joy:
