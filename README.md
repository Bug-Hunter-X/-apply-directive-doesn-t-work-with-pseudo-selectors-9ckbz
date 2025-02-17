# Tailwind CSS @apply Directive Bug with Pseudo-Selectors

This repository demonstrates a bug where Tailwind CSS's `@apply` directive fails to apply styles when used with classes containing pseudo-selectors (e.g., `:hover`, `:focus`, `:active`).

## Bug Description

The `@apply` directive does not correctly apply styles defined within classes that contain pseudo-selectors.  This results in missing hover effects, focus styles, or other dynamic styling.

## Reproduction Steps

1. Clone this repository.
2. Open `bug.css` to see the buggy code.
3. Build and run the application (if applicable).
4. Observe that the expected hover effects are not applied.

## Solution

To work around this issue, directly apply the individual Tailwind CSS utility classes instead of using `@apply` with classes containing pseudo-selectors.  See `bugSolution.css` for a corrected implementation.

## Additional Notes

This issue is specific to the usage of `@apply` with pseudo-selectors within the classes being applied.  Directly applying the utility classes will correctly produce the desired effects.