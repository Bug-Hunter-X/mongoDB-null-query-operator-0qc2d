# MongoDB $in operator with only null values
This repository demonstrates a common error when using the `$in` operator in MongoDB queries.  Specifically, when an array passed to `$in` contains only `null` values, the query returns no results, even if documents have null values for the specified field.

The `bug.js` file shows the incorrect implementation. The `bugSolution.js` shows the correct implementation using direct comparison for `null` values.