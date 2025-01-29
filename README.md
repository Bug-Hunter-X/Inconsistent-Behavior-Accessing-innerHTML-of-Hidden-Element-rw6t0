# Inconsistent Behavior Accessing innerHTML of a Hidden Element

This repository demonstrates an uncommon bug related to accessing the `innerHTML` property of a hidden HTML element. The bug exhibits inconsistent behavior across different browsers, making it difficult to debug.

## The Bug

The core issue lies in accessing the `innerHTML` property of an element after setting its `display` style to `"none"`. While this might work in some browsers without issues, others might throw errors or return unexpected results. This inconsistency makes the error hard to track down. The provided HTML file shows how this issue can be triggered by hiding an element and then attempting to access its `innerHTML`.

## Solution

The solution involves checking if the element is visible before attempting to access `innerHTML`.  This ensures consistent behavior across different browsers and prevents errors.