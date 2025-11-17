# CCS- CSS Animations Research

## What are CSS Animations?

CSS animations allow you to animate transitions from one CSS style configuration to another. They consist of two components:
1. **Style describing the CSS animation** - defined using the `@keyframes` rule
2. **CSS properties** - that assign the animation to specific elements

## How CSS Animations are Included in a Web Page

CSS animations can be included in web pages in three ways:

### 1. Inline Styles (Not Recommended)
```html
<div style="animation: slide 2s ease-in-out;">Content</div>
```

### 2. Internal CSS (Within `<style>` tags)
```html
<style>
  @keyframes slide {
    from { transform: translateX(0); }
    to { transform: translateX(100px); }
  }
  .animated-element {
    animation: slide 2s ease-in-out;
  }
</style>
```

### 3. External CSS File (Best Practice)
```html
<link rel="stylesheet" href="styles.css">
```

## Key Concepts

### @keyframes Rule
Defines the animation sequence by specifying CSS styles for various points during the animation:
```css
@keyframes animationName {
  0% { /* start state */ }
  50% { /* middle state */ }
  100% { /* end state */ }
}
```

### Animation Properties
- `animation-name`: Name of the @keyframes animation
- `animation-duration`: How long the animation takes
- `animation-timing-function`: Speed curve (ease, linear, ease-in, ease-out, cubic-bezier)
- `animation-delay`: Delay before animation starts
- `animation-iteration-count`: Number of times to repeat (or infinite)
- `animation-direction`: Direction (normal, reverse, alternate)
- `animation-fill-mode`: Style when animation is not playing (forwards, backwards, both)
- `animation-play-state`: Whether animation is running or paused

### Shorthand Syntax
```css
animation: name duration timing-function delay iteration-count direction fill-mode;
```

## Example Implementation

See `animation-example.html` for a working demonstration that includes:
- Fade-in animation
- Sliding animation
- Rotating animation
- Bounce effect
- Color changing animation

All animations demonstrate different timing functions and properties.
<img width="1221" height="2000" alt="image" src="https://github.com/user-attachments/assets/b1d9eda3-e3f2-4a5f-bbcb-56a539be39f8" />

