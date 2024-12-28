# CSS Calc() Function Unit Inconsistency

This repository demonstrates an uncommon bug related to the `calc()` function in CSS.  The bug arises from inconsistent unit handling when subtracting a unitless number from a percentage value within the `calc()` function. Some browsers may not interpret this correctly.

The `bug.css` file contains the buggy code, while `bugSolution.css` provides the corrected version.

## Bug Description

The original CSS code attempts to set width and height using `calc()`, but fails to maintain unit consistency leading to rendering issues in some browsers.  This is an uncommon error that developers might overlook.

## Solution

The solution involves ensuring that all values within the `calc()` function have consistent units. By adding units to the subtracted numerical values, consistent and predictable rendering can be obtained.