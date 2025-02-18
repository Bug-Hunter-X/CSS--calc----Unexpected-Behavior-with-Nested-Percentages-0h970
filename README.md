# CSS `calc()` Unexpected Behavior with Nested Percentages

This repository demonstrates an uncommon error when using the `calc()` function in CSS with nested elements and percentages. The issue arises from how CSS resolves percentage values within nested contexts.  The child element's width calculation is relative to its parent, not the grandparent, leading to unexpected results. 

## Reproduction

1. Clone the repository.
2. Open `index.html` (or any HTML file referencing the CSS files). 
3. Observe the unexpected width of the child element.

## Solution

Refer to `bugSolution.css` for a demonstration of how to mitigate this behavior, possibly by explicitly using absolute units, or by restructuring the CSS to avoid using nested percentages with `calc()`.