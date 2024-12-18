# Unexpected Behavior of :has() with Pseudo-elements

This repository demonstrates an uncommon CSS bug related to the `:has()` pseudo-class and its interaction with pseudo-elements (`::before`, `::after`).  The issue occurs in some browsers where `:has()` does not correctly recognize pseudo-elements as children.  The `bug.css` file contains the problematic code, while `bugSolution.css` provides alternative approaches to achieve the intended styling.

**Problem:**
The `:has()` selector is used to target parent elements based on the presence of specific child elements.  However, this example shows that its behavior with pseudo-elements is inconsistent across browsers, potentially causing unexpected styling issues.

**Solution:**
The suggested workaround in `bugSolution.css` uses a more robust selection strategy, avoiding reliance on `:has()` with pseudo-elements.

**Browser Compatibility:**
The inconsistency primarily affects certain older or less widely-used browsers.  It's important to thoroughly test your CSS across different browsers to ensure consistent styling.