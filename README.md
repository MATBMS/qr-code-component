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

![](./images/preview.jpg)

### Links

- Repository URL: [https://github.com/MATBMS/qr-code-component](https://github.com/MATBMS/qr-code-component)
- Live Site URL: [https://matbms.github.io/qr-code-component/](https://matbms.github.io/qr-code-component/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

#### `min-height: 100vh` and `100dvh`

To center the card vertically, `.page` must be at least as tall as the screen. I used `min-height` instead of `height` so the page can still grow if the content is taller (for example on a very small screen).

```css
.page {
  min-height: 100vh;
  min-height: 100dvh;
}
```

- `vh` is 1% of the viewport height. On mobile browsers, `100vh` is measured as if the address bar were hidden, so the page ends up taller than the visible area and the card is not truly centered (or a scrollbar appears).
- `dvh` ("dynamic viewport height") follows the visible area as the address bar shows or hides, so `100dvh` always matches what the user actually sees.
- I kept both lines. A browser that doesn't understand `dvh` ignores that line and keeps `100vh`, so it's a safe fallback.
- It only works well with `box-sizing: border-box`: otherwise the page padding is added on top of 100% of the height and creates a scrollbar.

### AI Collaboration

This project is **AI-driven**: I built it together with [Claude](https://claude.com/claude-code) (Claude Code), which acted both as the coder and as a mentor.

Claude wrote the code in small steps and explained every line, and I validated and understood each step before moving on. The goal was not to get the solution handed to me, but to learn pure HTML, CSS and JavaScript (no libraries, no frameworks) while practicing an AI-driven development workflow.
