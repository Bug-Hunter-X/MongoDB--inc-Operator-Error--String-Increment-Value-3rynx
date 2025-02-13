# MongoDB $inc Operator Error: String Increment Value

This repository demonstrates an example of an uncommon error in MongoDB update queries involving the `$inc` operator.  The error arises from using a string instead of a number as the increment value.

## Bug Description
The provided code attempts to increment the `count` field by '1' (a string).  MongoDB's `$inc` operator requires a numeric value for the increment.  This results in unexpected behavior, possibly leaving the field unchanged or throwing an error.

## Solution
The solution is to provide a numeric value to the `$inc` operator, using the correct data type.  The corrected query uses the number 1 to increment the count field.