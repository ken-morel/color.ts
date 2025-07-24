# color.ts

This project is a TypeScript rewrite and modernization of the original `w3color.js` library from w3schools. The original JavaScript code has been refactored into a TypeScript class named `Color`, providing a robust and type-safe way to work with colors.

## Overview

The `Color` class encapsulates color data and provides a rich API for color conversions and manipulations. It supports various color models, including:

*   **RGB / RGBA** (Red, Green, Blue)
*   **HSL / HSLA** (Hue, Saturation, Lightness)
*   **HWB / HWBA** (Hue, Whiteness, Blackness)
*   **CMYK** (Cyan, Magenta, Yellow, Black)
*   **NCol** (Natural Color System)
*   **Hexadecimal**
*   **Color Names**

## Features

*   **Parsing:** Create `Color` objects from CSS color strings in any of the supported formats (e.g., `"rgb(255, 0, 0)"`, `"#ff0000"`, `"red"`).
*   **Conversion:** Easily convert a `Color` object to any of the supported string formats (e.g., `toRgbString()`, `toHexString()`, `toHslString()`).
*   **Manipulation:** Methods to adjust color properties, such as `lighter()` and `darker()`.
*   **Utilities:** Helper functions for color-related calculations, like checking if a color is dark.
*   **Type-Safe:** Written in TypeScript to provide static typing and improved developer experience.

## Usage

To use the `Color` class, you can import it and create a new instance with a color string:

```typescript
import Color from './color';

const myColor = new Color('red');

console.log(myColor.toRgbString()); // "rgb(255, 0, 0)"
console.log(myColor.toHexString()); // "#ff0000"

const lighterRed = myColor.lighter(20);
console.log(lighterRed.toHexString());
```

This project aims to provide a more modern and maintainable version of the original w3schools color library, making it suitable for use in TypeScript-based projects.