# MongoDB $inc Operator with String Argument

This repository demonstrates a common yet subtle error in MongoDB queries when using the `$inc` operator with a string value instead of a numeric value.

The `bug.js` file contains the erroneous code, which attempts to increment the `count` field using a string '1'. This results in the field's value not being updated as expected.  The correct approach is to always supply a numerical value to `$inc`. 

The `bugSolution.js` file shows the corrected code, ensuring proper increment of the numeric value using the $inc operator. 

## How to reproduce the bug:
1. Make sure you have a MongoDB instance running. 
2. Execute `bug.js`. 
3. Observe the result. 
4. Execute `bugSolution.js` to see the corrected behavior. 
