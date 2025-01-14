# MongoDB Aggregation Pipeline: Incorrect use of $inc operator

This repository demonstrates an uncommon error in MongoDB aggregation pipelines involving the `$inc` operator.  The `$inc` operator is designed to increment a field's value.  However, it's crucial to use it correctly within the context of the aggregation pipeline stages, particularly within the `$group` stage.

The `bug.js` file showcases the incorrect usage which results in an error or unexpected output. The corrected implementation is provided in `bugSolution.js`.

## Reproducing the Error

1.  Clone this repository.
2.  Connect to your MongoDB instance.
3.  Execute the code in `bug.js`.
4.  Observe the error or unexpected results.

## Solution

The correct way to use the `$inc` operator in the context of an aggregation pipeline is to place it within the `$group` stage and use it to increment fields within each grouped document.  This is demonstrated in `bugSolution.js`.

This example highlights the importance of understanding the proper application of MongoDB aggregation pipeline operators to ensure accurate and expected results.