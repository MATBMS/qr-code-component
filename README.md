# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H).

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [AI Collaboration](#ai-collaboration)

## Overview

### Screenshot

![Screenshot Preview](./docs/preview.jpg)

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

### What I learned

#### Import a local font

To import a local TrueType font (`.ttf`) into my CSS using the `@font-face` rule:

```css
@font-face {
  font-family: "Outfit";
  src: url("./fonts/Outfit-Regular.ttf") format("truetype");
  font-weight: 400;
  font-style: normal;
  font-display: swap;
}

@font-face {
  font-family: "Outfit";
  src: url("fonts/Outfit-Bold.ttf") format("truetype");
  font-weight: 700;
  font-style: normal;
  font-display: swap;
}
```

Once imported, we can apply the font name to any element just like standard fonts:

```css
.text-preset-1 {
  font-family: "Outfit";
  font-weight: 700; /* Uses Outfit-Bold.ttf */
}

.text-preset-2 {
  font-family: "Outfit";
  font-weight: 400; /* Uses Outfit-Regular.ttf */
}
```

Because both share the same family name, we only need to declare the font family once. The browser handles switching between the regular and bold files based on the style.

### AI Collaboration

No AI was used during this project.
