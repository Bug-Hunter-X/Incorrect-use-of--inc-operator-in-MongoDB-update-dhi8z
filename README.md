# Incorrect use of $inc operator in MongoDB update
This example demonstrates an uncommon error when using the `$inc` operator in MongoDB update operations.  The `$inc` operator is used to increment a numerical field.  However, if a string is passed as the increment value, it will not perform a numerical increment, and instead may lead to unexpected behavior or errors.

The file `bug.js` shows the incorrect usage, and `bugSolution.js` provides the correct implementation.  Care should be taken to always provide a numerical value to the `$inc` operator.