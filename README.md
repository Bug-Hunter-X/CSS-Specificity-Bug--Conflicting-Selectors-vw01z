# CSS Specificity Bug: Conflicting Selectors

This repository demonstrates an uncommon bug related to CSS specificity.  The `bug.css` file contains CSS code with conflicting selectors that lead to unexpected results depending on the HTML structure. The `bugSolution.css` file provides a solution for resolving the conflict.

The bug arises from a misunderstanding of how CSS specificity works when dealing with nested elements and potentially conflicting selectors. The core issue is that selectors with higher specificity override selectors with lower specificity.

## Bug Description

The main issue lies in the conflicting styles applied to paragraph elements within a `div`.  Depending on the HTML context, either the `color: blue;` or the `color: red;` rule might unexpectedly take precedence. This can make the styling unpredictable and difficult to debug.