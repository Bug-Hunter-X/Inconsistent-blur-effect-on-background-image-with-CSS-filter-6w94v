# Inconsistent Blur Effect on Background Image with CSS filter

This repository demonstrates a bug related to applying the CSS `filter: blur()` property to an element with a background image. The expected behavior is a consistent blur effect applied across the entire element, including the background image. However, the actual behavior shows an inconsistent blur, potentially affecting only the content or the background separately.

## Bug Report

The bug occurs when you try to blur an element that contains a background image using the `filter: blur()` property. Instead of a uniform blur across both the element's content and the background image, only one of them might be blurred, or the blur effect is partially applied, producing unexpected visual artifacts.

## Steps to Reproduce

1. Open the `bug.css` and `index.html` files.
2. Observe the rendered element with the background image and blur filter applied.
3. Note the inconsistent or unexpected blur effect.

## Solution

The `bugSolution.css` file provides a workaround. Consider setting the `filter` property on an element that completely encloses both the background and content and acts as a wrapper for the content to produce the correct blur effect.

## Additional Notes

This bug might be related to browser compatibility or the specific way the background image is handled by the browser's rendering engine. The solution provided might not be applicable in all cases and might require further investigation depending on your specific setup.