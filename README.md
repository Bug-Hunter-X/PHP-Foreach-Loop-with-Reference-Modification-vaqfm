# PHP Foreach Loop with Reference Modification Bug

This repository demonstrates a subtle bug related to using references in PHP's `foreach` loop.  Incorrect usage can lead to unexpected results when modifying array elements within the loop.

The `bug.php` file contains the erroneous code. The `bugSolution.php` file offers a corrected version.

## Bug Description

In PHP, passing an array by reference to a function using `&` allows modification within the function to affect the original array. However, the way references work within `foreach` loops needs careful consideration. When a reference is created inside `foreach`, changes made might affect the iteration process itself.

## Solution

The solution involves understanding how to correctly manage references within `foreach` to avoid unexpected outcomes.   The corrected version in `bugSolution.php` avoids the issue.