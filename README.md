# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). 
## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)
- [Acknowledgments](#acknowledgments)


## Overview


### Screenshot

![](./images/Screenshot.png)

### Links

-  [Solution URL:](https://github.com/frkanyilmaz2/nft-preview)
-  [Live Site URL:](https://frkanyilmaz2.github.io/nft-preview/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

I was feeling addictive to 
```
random-name{
  position:absolute;
  left:50%;
  top: 50%;
  transform:translate(-50%;-50%)
}
```
This code makes the .random-name both horizontally and vertically centered. I used this so much that it starting to feel like cheesy. So I tried a different approach and put .random-name inside a container then used flex to center everything. I'll keep using this strategy until it gives cheese vibe.

I also didn't know how to add an overlay to an image. With this project I learned that I can achieve this with this line 

```
.overlay {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  background-color: rgba(0, 255, 248, 0.5);
  border-radius: 15px;
  width: 100%;
  height: 100%;
  opacity: 0;
  transition: opacity 0.3s ease;
  background-size: cover;

  display: flex;
  justify-content: center;
  align-items: center;
}
```

Basically put base img and overlay into a container. And then put them on top of each other. When hovered opacity of the overlay becomes 1 and shows itself. 