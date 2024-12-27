# MongoDB $inc Operator Error

This repository demonstrates a common error when using the `$inc` operator in MongoDB update queries.  The `$inc` operator is used to increment or decrement a numeric field by a specified value.  However, the value provided must be a number; providing a string results in unexpected behavior. 

The `bug.js` file shows the erroneous code, while `bugSolution.js` provides the corrected version.

## Bug
The original code incorrectly uses a string ('1') instead of a number (1) as the increment value. This leads to the field not being incremented correctly or even an error depending on the MongoDB version and configuration.

## Solution
The corrected code uses the correct numeric value (1) to correctly increment the field.