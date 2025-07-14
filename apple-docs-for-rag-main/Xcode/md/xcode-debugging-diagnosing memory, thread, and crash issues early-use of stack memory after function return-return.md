

- Xcode
- Debugging
- Diagnosing memory, thread, and crash issues early
-  Use of stack memory after function return 

Article

# Use of stack memory after function return

Detects when you access stack variable memory after its declaring function returns.

## Overview

Use this check to detect access to a stack variable that a function declares after that function returns. Attempting to access stack memory in this manner can lead to crashes, or result in unpredictable behavior. Available in Xcode 9 and later.

Note

This check is in a disabled state by default. You can enable it under the Address Sanitizer option in the Edit Scheme dialogue.

### Use of stack memory after return in C

In the following example, the `integer_pointer_returning_function` function returns a pointer to a stack variable, and there’s an attempt to access the memory of the returned pointer:

```
int *integer_pointer_returning_function() {
    int value = 42;
    return &value;
}

int *integer_pointer = integer_returning_function();
*integer_pointer = 43; // Error: invalid access of returned stack memory
```

#### Solution

Use pointer arguments to allow a function to return values by reference.

## See Also

### Address Sanitizer

Use of deallocated memory

Detects the use of deallocated memory.

Deallocation of deallocated memory

Detects attempts to free deallocated memory.

Deallocation of nonallocated memory

Detects attempts to free nonallocated memory.

Use of out-of-scope stack memory

Detects access to variables outside of their declared scope.

Overflow and underflow of buffers

Detects when you access memory outside of a buffer’s boundaries.

Overflow of C++ containers

Detects when you access a C++ container outside its bounds.

