# CSS Specificity Conflict Bug
This repository demonstrates a common issue in CSS: specificity conflicts that lead to unexpected styling.

## Description
The bug involves a specificity conflict between a general style rule for `h1` elements and a more specific style rule for `h1` elements within a `.container` class.  The general rule unintentionally overrides the more specific rule.

## How to Reproduce
1. Open `bug.css`.
2. Observe that the `h1` element inside the `.container` unexpectedly displays blue text instead of red, despite the more specific style rule.

## Solution
The solution, found in `bugSolution.css`, addresses the specificity conflict by increasing the specificity of the more specific rule or overriding the general rule by using `!important`.  The latter approach is generally discouraged due to its potential for cascading issues.