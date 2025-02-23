# Uncommon HTML and JavaScript Bugs

This repository demonstrates a couple of uncommon errors that can occur when working with HTML and JavaScript.

## Bug 1: Adding Event Listener to Non-Existing Element

The first bug showcases the issue of trying to add an event listener to an element that hasn't been parsed by the browser yet.  This often leads to a `TypeError: Cannot read properties of null (reading 'addEventListener')`.

## Bug 2: Using a Reserved Keyword as an ID

The second bug highlights the problem of using a reserved keyword (like `class`) as an element's ID. This is generally bad practice, leading to unexpected behavior and making your code harder to debug.

## Solution

The solution involves ensuring the element exists before adding the event listener (using `DOMContentLoaded` or checking the element's existence before adding listener). Also, the reserved keyword should be replaced with a suitable valid id.  See the `bugSolution.html` file for the corrected code.