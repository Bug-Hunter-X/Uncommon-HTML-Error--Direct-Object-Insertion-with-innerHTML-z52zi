# Uncommon HTML Error: Direct Object Insertion with innerHTML

This repository demonstrates an uncommon error in HTML related to the misuse of `innerHTML` when attempting to insert a JavaScript object directly into the DOM.  The error leads to unexpected behavior.

The `bug.html` file shows the incorrect implementation. The `solution.html` file provides the corrected code.

## Bug Description
The issue lies in the direct assignment of a JavaScript object to `innerHTML`.  `innerHTML` expects a string; assigning an object results in an empty output or a runtime error, depending on the browser's behavior.

## Solution
The correct approach is to first convert the JavaScript object into a string representation (e.g., using `JSON.stringify()`) before assigning it to `innerHTML`.  This ensures that the browser can correctly interpret and display the data.