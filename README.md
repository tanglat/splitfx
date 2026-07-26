# SplitFX

A JavaScript plugin for splitting and animating text.

## Links

- **[Website](https://tanglat.github.io/splitfx/)**
- **[Demo Projects](https://tanglat.github.io/splitfx/#demo-projects)**
- **[Demos](https://tanglat.github.io/splitfx/demos/)**
- **[Documentation](https://tanglat.github.io/splitfx/docs/latest/)**
- **[SplitFX Studio](https://tanglat.github.io/splitfx/studio/)**
- **[Licensing](https://tanglat.github.io/splitfx/license.html)**

## Overview

SplitFX is a JavaScript plugin that splits the text of HTML elements into individual units (characters and words) and animates them.

## Features

- **Animate by Chars or Words**  
    You can choose to animate text by chars or words.

- **Multiple Trigger Options**  
    Animate HTML elements' text in and out on scroll, window load, hover, or click.

- **Full Animation Control**  
    Full control over animation timing, stagger, stagger direction, and easing.

- **A Variety of Built-in Animations**  
    Choose from a variety of built-in animations such as fade, zoom in, and more.

- **Use Your Custom Animations**  
    Build and use your own animations to create text effects tailored to your needs.

- **Different Stagger Directions**  
    Control the animation flow with stagger directions like forward, backward, center-out, random, and more.

- **Sequential Text Animations**  
    Run text animations step by step in a defined sequence, just like the hero of this page and each demo project.

- **Supports Nested Elements**  
    Split and animate the text of HTML elements even when they contain nested elements.

- **Easy to Use**  
    A set of convenience methods that make SplitFX easier to use.

- **No Dependencies**  
    Built specifically for text animations with zero external dependencies.

- **SEO-friendly**  
    Works on the text you already have in your HTML, so search engines can read it.

## Resources

- **[Demos](https://tanglat.github.io/splitfx/demos/)**  
    Get inspired by ready-made text animation demos.

- **[Docs](https://tanglat.github.io/splitfx/docs/latest/)**  
    Clear and structured docs to help you understand and use SplitFX.

- **[Studio](https://tanglat.github.io/splitfx/studio/)**  
    Build, test, and export animations with the SplitFX Studio.

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

For complete documentation, more demos, visit our **[Website](https://tanglat.github.io/splitfx/)**.