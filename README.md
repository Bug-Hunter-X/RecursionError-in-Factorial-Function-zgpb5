# RecursionError in Factorial Function

This repository demonstrates a common error in recursive functions: improper handling of base cases, leading to infinite recursion and a `RecursionError`. The `factorial_bug.py` file contains the erroneous code, while `factorial_solution.py` provides a corrected version.

## Bug Description:

The original `factorial` function does not check for negative input.  When a negative number is passed, the recursion continues indefinitely until Python's maximum recursion depth is exceeded, causing the error. 

## Solution:

The solution adds an explicit check for negative input, raising a ValueError if encountered. Otherwise, the function proceeds as before, correctly calculating factorials for non-negative integers.