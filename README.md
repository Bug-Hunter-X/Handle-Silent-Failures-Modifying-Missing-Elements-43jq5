# Silent Failure: Modifying Non-Existent Element's innerHTML

This example demonstrates a subtle bug in HTML where attempting to manipulate the `innerHTML` property of a non-existent element results in no error but also no visible change. The code silently fails, leading to unexpected behavior.

## Bug Description:

The `bug.html` file contains JavaScript code that tries to change the `innerHTML` of an element with the ID 'nonExistentElement'. Since this element doesn't exist in the HTML structure, the operation fails without throwing an error, preventing the intended text from appearing.

## Solution:

The `bugSolution.html` file shows the solution:  First, verify the existence of the element using `getElementById`. If the element exists, *then* modify its `innerHTML`.  This prevents the silent failure.

## How to run:
1. Open bug.html and bugSolution.html in a web browser.
2. Observe the different behavior between the two files.