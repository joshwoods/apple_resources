

- Xcode
- Debugging
- Diagnosing memory, thread, and crash issues early
-  Use of out-of-scope stack memory 

Article

# Use of out-of-scope stack memory

Detects access to variables outside of their declared scope.

## Overview

Use this check to detect when you access a variable outside of its scope. Attempting to access out-of-scope memory can result in unpredictable behavior. Available in Xcode 9 and later.

### Use of out-of-scope stack memory in C

In the following example, the code conditionally assigns the `pointer` variable to the return value of the `integer_returning_function` function, which it then accesses out of its declaration scope:

```
int *pointer = NULL;
if (bool_returning_function()) {
    int value = integer_returning_function();
    pointer = &value;
}
*pointer = 42; // Error: invalid access of stack memory out of declaration scope
```

#### Solution

Ensure you don’t access variables outside of their declared scope, or allocate memory using the `malloc` function.

## See Also

### Address Sanitizer

Use of deallocated memory

Detects the use of deallocated memory.

Deallocation of deallocated memory

Detects attempts to free deallocated memory.

Deallocation of nonallocated memory

Detects attempts to free nonallocated memory.

Use of stack memory after function return

Detects when you access stack variable memory after its declaring function returns.

Overflow and underflow of buffers

Detects when you access memory outside of a buffer’s boundaries.

Overflow of C++ containers

Detects when you access a C++ container outside its bounds.

