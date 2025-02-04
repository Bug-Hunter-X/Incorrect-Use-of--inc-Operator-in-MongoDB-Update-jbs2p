# Incorrect Use of $inc Operator in MongoDB

This example demonstrates a common error when using the `$inc` operator in MongoDB updates.  The `$inc` operator is designed to increment numeric fields; using it with a string value results in an error.

The `bug.js` file shows the incorrect usage. The `bugSolution.js` file provides the corrected code.

## Bug
The bug arises from trying to increment a field with a string value. MongoDB's `$inc` operator requires a numeric value.  This incorrect usage leads to an error. 

## Solution
The solution involves ensuring the field is of numeric type (either NumberInt or NumberLong) before applying the `$inc` operator.