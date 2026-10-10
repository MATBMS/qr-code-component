# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H).

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Features](#features)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [AI Collaboration](#ai-collaboration)

## Overview

### Screenshot

#### Preview

![Screenshot Preview](./docs/preview.jpg)

#### Desktop Screenshot

![Desktop Screenshot](./docs/desktop-screenshot.png)

#### Desktop On Hover Screenshot

![Desktop On Hover Screenshot](./docs/desktop-hover-screenshot.png)

### Features

**As a** User<br>
**I need to** be able to zoom on the QR Code<br>
**So that I** can scan the QR code easily

### Links

- Repository URL: [GitHub Repo](https://github.com/MATBMS/qr-code-component)
- Live Site URL: [GitHub Page](https://matbms.github.io/qr-code-component/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
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
