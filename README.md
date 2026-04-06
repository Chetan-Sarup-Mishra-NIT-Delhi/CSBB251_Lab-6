# Debugging C Programs Using GDB (GNU Debugger)

## Introduction

Debugging is an essential step in software development that helps programmers identify and fix errors in their code. One of the most powerful debugging tools for C and C++ programs is **GDB (GNU Debugger)**.

GDB allows developers to:
- Run programs step by step
- Inspect variables
- Set breakpoints
- Monitor memory and registers
- Track program execution flow

This document explains how to use **GDB** using the **OnlineGDB platform**, demonstrated with the example program shown in the screenshots.

---

# Example Program Used

The following C program demonstrates the use of pointers and basic variable operations. The assembly code is in the output image file, illustrating the addressing modes in use. 

```c
#include <stdio.h>

int global_var=100;

int main()
{
    int a=50;
    int b=a+10;
    int c=global_var;
    int *ptr=&c;
    int d=*ptr;
    d=*ptr++;
    int arr[5]={10, 20, 30, 40, 50};
    int e=arr[2];
    printf("Values: %d, %d, %d, %d, %d\n", a, b, c, d, e);
    return 0;
};
