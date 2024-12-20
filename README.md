# Uninitialized Pointer Dereference in C

This repository demonstrates a common but subtle error in C: dereferencing an uninitialized pointer.  Uninitialized pointers can lead to unpredictable behavior and crashes. The example code showcases how this can happen and provides a corrected version.

## Bug Description

The `bug.c` file contains code that attempts to dereference a pointer (`ptr`) without first assigning it a valid memory address. This results in undefined behavior – the program might crash, produce incorrect results, or appear to work correctly but fail under different circumstances.

## Solution

The `bugSolution.c` file provides a corrected version.  Before dereferencing `ptr`, the code explicitly assigns it the address of the variable `x` using the `&` operator.