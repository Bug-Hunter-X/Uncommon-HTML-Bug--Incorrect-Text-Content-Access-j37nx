# Uncommon HTML Bug: Incorrect Text Content Access

This repository demonstrates a common but easily missed bug in HTML involving how to properly access text content from a div element. The bug involves attempting to use `textContent` on a div that contains other elements when you actually want the complete inner HTML of that div. 

## Bug Description

The code attempts to access the text content of a div using `textContent`. However, this only returns the text content of the *first child* element of the div, rather than the entire content, which results in an unexpected output if the div has multiple child elements.  This behavior can be easily confused with the `innerHTML` property which correctly returns all inner content of a tag.

## Solution

The correct way to retrieve the content of a div, including any nested elements, is to use the `innerHTML` property.