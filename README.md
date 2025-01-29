# Ada Shallow Copy Bug
This example demonstrates a common issue in Ada related to array copying.  Ada, by default, performs a shallow copy of arrays, meaning both variables point to the same underlying memory location. Changes made through one variable affect the other.

The provided `bug.ada` file shows a scenario where modifying one array unintentionally modifies another. The `bugSolution.ada` file presents a corrected version that uses a deep copy using an explicit loop.

## How to reproduce
1. Compile and run the `bug.ada` code.
2. Observe the unexpected behavior of array B being modified although only array A was updated directly.
3. Compare the output of `bug.ada` and `bugSolution.ada` to understand the difference.