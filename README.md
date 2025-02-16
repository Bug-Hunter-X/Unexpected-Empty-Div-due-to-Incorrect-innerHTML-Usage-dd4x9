# Uncommon HTML Bug: Incorrect innerHTML Usage

This repository demonstrates an uncommon bug in HTML related to the use of `innerHTML`.  The `innerHTML` property expects a string; attempting to set it to a JavaScript object will result in an empty element, not the expected output. 

The `bug.html` file shows the erroneous code, while `bugSolution.html` provides the corrected version.

## Bug
The bug lies in the misuse of the `innerHTML` property in JavaScript. When we try to assign a JavaScript object to the `innerHTML` property it does not render anything.

## Solution
The solution is to convert the JavaScript object to a string before assigning it to the `innerHTML` property.  JSON.stringify() is a useful method for this purpose. 