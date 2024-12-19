# Ada Off-by-One Error Example
This example demonstrates a common off-by-one error in Ada programming.  Ada arrays are 1-based, meaning the first element is at index 1, not 0.  Incorrectly assuming a 0-based index will lead to a runtime error.  The solution shows how to correctly iterate through the array's elements.

## Bug
The `bug.ada` file contains code with an error that attempts to access an array element outside of its valid index range, leading to a `Constraint_Error` exception. 

## Solution
The `bugSolution.ada` file provides a corrected version of the code. The loop now correctly iterates from the lower bound (1) to the upper bound of the array.