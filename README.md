# Tailwind CSS @apply Directive Issue with Pseudo-Class Selectors

This repository demonstrates a bug where Tailwind CSS's `@apply` directive doesn't correctly handle pseudo-class selectors like `:hover` and `:focus` when applied within a class.  The `bug.css` file showcases the problem, and `bugSolution.css` offers a workaround.

## Bug Description

When using `@apply` to include a class with a pseudo-class selector, the expected styles are not applied.  This leads to missing hover effects, focus states, or other styles dependent on pseudo-class selectors.

## Solution

The issue is that `@apply` was designed primarily to work with static classes.  While the solution may not be perfect, it is best to avoid using the `@apply` directive with pseudo classes to solve the problem.

## How to Reproduce

1. Clone this repository.
2. Include `bug.css` in your project.
3. Observe that the hover effect doesn't work.
4. Replace with `bugSolution.css` to see that it solves the issue.