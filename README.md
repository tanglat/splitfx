# SplitFX

JavaScript text animation plugin that splits text into characters and words and animates them.

## Links

- **[Website](https://splitfx.pages.dev/)**
- **[Demo Projects](https://splitfx.pages.dev/#demo-projects)**
- **[Demos](https://splitfx.pages.dev/demos/)**
- **[Documentation](https://splitfx.pages.dev/docs/latest/)**
- **[SplitFX Studio](https://splitfx.pages.dev/studio/)**
- **[Licensing](https://splitfx.pages.dev/license)**

## Overview

SplitFX is a JavaScript text animation plugin that splits the text of HTML elements into individual units (characters and words) and animates them.

## Features

- **Animate Text by Chars or Words**  
    You can choose to animate text by chars or words.

- **Multiple Trigger Options**  
    Animate HTML elements' text in and out on scroll, window load, hover, or click.

- **Full Animation Control**  
    Full control over animation timing, stagger, stagger direction, and easing.

- **A Variety of Built-in Text Animations**  
    Choose from a variety of built-in text animations such as fade, typeWriter, and more.

- **Use Your Custom Text Animations**  
    Build and use your own animations to create text animations tailored to your needs.

- **Different Stagger Directions**  
    Control the animation flow with stagger directions such as forward, backward, centerOut, random, and more.

- **Sequential Text Animations**  
    Run text animations step by step in a defined sequence, just like the hero of this page.

- **Supports Nested Elements**  
    Split and animate the text of HTML elements even when they contain nested elements.

- **Easy to Use**  
    A set of convenience methods that make SplitFX easier to use.

- **No Dependencies**  
    Built specifically for text animations with zero external dependencies.

## Resources

- **[SplitFX Demos](https://splitfx.pages.dev/demos/)**  
    Get inspired by ready-made text animation demos built with SplitFX.

- **[SplitFX Documentation](https://splitfx.pages.dev/docs/latest/)**  
    Find everything you need to create text animations with SplitFX.

- **[SplitFX Studio](https://splitfx.pages.dev/studio/)**  
    Create, customize, and preview text animations with SplitFX Studio.

## Quick Start

### Include the script:

```html
<script src="https://cdn.jsdelivr.net/npm/@tanglat/splitfx@1/dist/umd/splitfx.min.js"></script>
```

### Example Usage:

```js
// Select the HTML element you want to animate
const heading = document.querySelector(".heading");

// Create a new SplitFX instance with your configuration options
const textAnimator = new SplitFX({
    in: {
        mode: "chars",
        includeSpaces: true,
        animation: "fadeRight",
        duration: 500,
        easing: "ease",
        stagger: 50,
        staggerDir: "forward",
        delay: 0
    },
    out: {
        mode: "words",
        duration: 0,
        stagger: 0
    },
    tagName: "span"
});

// Animate the text of the given element every time it enters the viewport during scrolling
textAnimator.animateOnScroll(heading);
```

For complete documentation, more demos, visit our **[Website](https://splitfx.pages.dev/)**.