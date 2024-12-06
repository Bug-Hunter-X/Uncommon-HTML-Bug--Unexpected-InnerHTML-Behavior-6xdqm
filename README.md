# Uncommon HTML Bug: Unexpected InnerHTML Behavior

This repository demonstrates an uncommon bug related to the use of `innerHTML` in HTML.  The bug arises from incorrectly appending content using `innerHTML`, which can lead to unexpected behavior and potential issues with element ordering and layout.  The solution demonstrates a more robust approach to appending content, ensuring correct functionality.

## Bug Description
The bug involves appending a new paragraph to a div using `innerHTML` by concatenating the new paragraph with the existing `innerHTML`. This approach is problematic as it doesn't guarantee the order of content or handle potential pre-existing content appropriately. The outcome might differ between browsers or even different versions of the same browser.

## Solution
The solution demonstrates a more robust approach using `insertAdjacentHTML`. This approach avoids the pitfalls associated with the direct manipulation of `innerHTML`. It provides a more controlled and reliable method for appending elements to HTML structures.

## How to reproduce the bug
1. Open `bug.html` in your web browser.
2. Observe the unexpected behavior in the layout or content.