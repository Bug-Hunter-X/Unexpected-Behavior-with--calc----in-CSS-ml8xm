# Unexpected Behavior with `calc()` in CSS

This repository demonstrates common yet subtle errors encountered when using the `calc()` function in CSS, specifically focusing on scenarios within flexbox and unit handling.

## Bug Description
The `calc()` function, while powerful, can lead to unexpected results if not used carefully. The primary issues highlighted here are:

1. **Incorrect `calc()` usage within flexbox:** If `calc()` is used to determine the width or height of an element within a flexbox container without explicitly defining the `width` property, unexpected layout may occur.
2. **Unit inconsistencies:** Errors arise from improper unit handling within `calc()` expressions.  Missing or inconsistent units prevent correct calculation.

## How to reproduce
1. Clone this repository.
2. Open `bug.css` to see the problematic code.
3. Open `bugSolution.css` to view the corrected implementation.

## Solution
The solution addresses both issues by:

1. Ensuring the `width` property is explicitly defined for elements using `calc()` within flexbox layouts.
2. Maintaining unit consistency throughout the `calc()` expressions, with explicit unit declaration for all values.
