# Uncommon HTML Bug: Accessing innerHTML of Non-Existent Element

This repository demonstrates an uncommon error that can occur when manipulating the DOM in HTML using JavaScript. The bug arises from attempting to access and modify the `innerHTML` property of an element that does not yet exist in the DOM.

## Bug Description
The `bug.html` file contains a script that tries to access and modify the `innerHTML` property of an element with the ID 'nonExistentElement'. Since this element doesn't exist at the time the script executes, it results in an error that prevents further script execution.

## Bug Solution
The `bugSolution.html` file provides a corrected version. The script checks for the element's existence using `document.getElementById()` before attempting to modify its `innerHTML`. If the element doesn't exist, a suitable alternative action (e.g., logging a message or creating the element) can be taken.

## How to Reproduce the Bug
1. Open `bug.html` in a web browser.
2. Observe the error message in the browser's developer console.
3. The expected outcome is that 'This text replaces the original content' should replace the text inside the div with id myDiv, however due to the prior error, this is not displayed.

## How to Run the Solution
1. Open `bugSolution.html` in a web browser.
2. The text within the div with id myDiv is properly updated.