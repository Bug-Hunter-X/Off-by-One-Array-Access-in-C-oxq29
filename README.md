# Off-by-One Array Access in C

This repository demonstrates a common off-by-one error in C, where an array index goes beyond the valid range.  The `bug.c` file contains the erroneous code, while `bugSolution.c` provides the corrected version.

**The Problem:**
The original code attempts to access `arr[5]` in an array declared as `arr[5]`.  Valid indices are 0 through 4. Accessing `arr[5]` leads to undefined behavior; it might crash, produce incorrect results, or seemingly work correctly – making it a particularly insidious bug.

**The Solution:**
The corrected code ensures that array accesses remain within the bounds 0 to 4.  It illustrates good programming practice for managing array indices.