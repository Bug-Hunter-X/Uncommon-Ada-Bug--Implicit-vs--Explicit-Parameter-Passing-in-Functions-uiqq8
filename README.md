# Uncommon Ada Bug: Implicit vs. Explicit Parameter Passing

This repository demonstrates a subtle bug that can occur in Ada related to function parameter passing. While not a common error, it highlights the importance of understanding implicit and explicit parameter associations.

## The Bug

The `Calculate_Area` function calculates the area of a rectangle. The `Main` procedure calls this function.  If you were to unintentionally switch the order of the parameters in the function call in `Main`, the program would still compile and run without reporting an error, but it would produce an incorrect result because of Ada's implicit parameter matching.  This can easily be avoided by using named parameters in the function call.

## The Solution

The solution is to always use named parameters when calling functions in Ada. This avoids ambiguity and makes the code more readable and maintainable. This makes it clear which parameter is assigned to which variable, preventing such unexpected results. 

## How to Run

1.  You'll need an Ada compiler (like GNAT). 
2.  Compile the Ada code in `bug.ada`. 
3.  Run the compiled executable.  Observe the output.
4.  Compile and run `bugSolution.ada` to see the solution in action.
