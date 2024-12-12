# MongoDB $inc operator type error in findAndUpdate
This example demonstrates a common error when using the `$inc` operator within MongoDB's `findOneAndUpdate` method.  The issue arises from providing a string value instead of a numeric value to the `$inc` operator, preventing the counter from incrementing correctly.

## Bug Description
The `$inc` operator is used to increment a numeric field in a MongoDB document.  This example shows the incorrect usage where the value provided to `$inc` is a string instead of a number. This leads to either a failure to update the document or unexpected results.

## Bug Solution
The corrected solution demonstrates the correct usage of `$inc` where the value to increment by is a number (integer or float) rather than a string.