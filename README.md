# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H).

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Features](#features)
  - [Extra feature](#extra-feature)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [AI Collaboration](#ai-collaboration)

## Overview

### Screenshot

![](./images/preview.jpg)

### Features

1. The challenge is to build out this QR code component and get it looking as close to the design as possible.

### Extra feature

### Links

- Repository URL: [GitHub](https://github.com/MATBMS/qr-code-component)
- Live Site URL: [Netlify](https://matbms-qr-code-component.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

#### Internal Fonts

The `@font-face` CSS at-rule specifies a custom font with which to display text; the font can be loaded from either a remote server or a locally-installed font on the user's own computer.

To make weights work correctly with variables, I structure your stylesheet like this:

```css
@font-face {
  font-family: "Outfit";
  src: url("./fonts/Outfit-Regular.ttf") format("tff");
  font-weight: 400;
}

@font-face {
  font-family: "Outfit";
  src: url("./fonts/Outfit-Bold.ttf") format("tff");
  font-weight: bold;
}
```

#### Custom Properties

**Custom properties** (sometimes referred to as **CSS variables** or **cascading variables**) are entities defined by CSS authors that represent specific values to be reused throughout a document.

```css
:root {
  /* color */
  --color-slate-900: #1f314f;
  --color-slate-500: #68778d;
  --color-slate-300: #d5e1ef;
  --color-white: #fff;
  /* spacing */
  --spacing-500: 40px;
  --spacing-300: 24px;
  --spacing-200: 16px;
}
```

Once the custom properties are set up on the `:root` element, I can access them anywhere in my project.

### AI Collaboration

No AI was used in this project.
