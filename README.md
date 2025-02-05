# CSS Specificity Bug

This repository demonstrates a subtle bug related to CSS specificity.  The bug involves unexpected style overrides due to the order of style declarations and the interaction between ID and class selectors.  The problem lies in the unexpected behavior when a later style with lower specificity overrides a more specific style due to the order of style declarations. This is an uncommon issue that highlights the complexity of CSS specificity and cascading.

## How to Reproduce

1. Clone this repository.
2. Open `bug.css` and `bugSolution.css`.
3. Observe the unexpected behavior of the CSS styles in `bug.css`.  The element should display green but unexpectedly displays red.
4. The `bugSolution.css` shows a corrected approach using proper specificity and avoiding order dependencies.

## Solution

The solution involves carefully ordering CSS rules to ensure that the most specific styles are applied correctly.  In this case, it was important to address the order of the selectors to enforce higher specificity.