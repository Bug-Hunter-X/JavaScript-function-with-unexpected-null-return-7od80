# JavaScript subtle bug: Unexpected null return
This repository demonstrates a subtle bug in a JavaScript function that unexpectedly returns null even when it shouldn't. The issue lies in the handling of null values. 
The `foo` function intends to return null only if either 'a' or 'b' is strictly equal to null. However, due to the loose equality check, it incorrectly returns null if either 'a' or 'b' is falsy. 
The solution addresses this by using strict equality (`===`) and explicitly checks for null or undefined separately. 