# Dangling Pointer Bug in C
This repository demonstrates a common yet dangerous bug in C programming: using a dangling pointer.  A dangling pointer points to memory that has been freed, leading to unpredictable behavior and program crashes.  This example showcases the issue and provides a solution.

## The Bug
The `bug.c` file contains code that allocates memory using `malloc`, assigns a value, frees the memory using `free`, and then attempts to access the freed memory again. This is the source of the dangling pointer.

## The Solution
The `bugSolution.c` file shows how to avoid this problem by setting the pointer to `NULL` after freeing the allocated memory. This makes it clear that the pointer no longer points to valid memory and prevents accidental access.