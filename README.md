# Uncommon HTML Bug: Incorrect ID Selector with Spaces

This repository demonstrates a subtle error that can occur in HTML when working with element IDs that contain spaces. The bug lies in attempting to select an element using `document.getElementById()` with an ID that has spaces.

## Bug Description
The provided `bug.html` file contains a `div` element with an ID that includes spaces: `my Div`. The JavaScript code attempts to change the inner HTML of this element using `document.getElementById("my Div")`. However, this approach will fail because spaces are invalid characters within an HTML ID.

## Bug Solution
The solution, shown in `bugSolution.html`, demonstrates the correct approach. The ID should be modified to be a single word (e.g., `myDiv`) without spaces, ensuring proper selection using `document.getElementById()`. Alternatively, if spaces are necessary in the ID, a different selector method (like `querySelector` with a more specific selector) would be required.