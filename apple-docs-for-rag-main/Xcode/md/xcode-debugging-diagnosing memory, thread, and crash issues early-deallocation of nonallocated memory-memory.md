

- Xcode
- Debugging
- Diagnosing memory, thread, and crash issues early
-  Deallocation of nonallocated memory 

Article

# Deallocation of nonallocated memory

Detects attempts to free nonallocated memory.

## Overview

Use this check to detect when you call `free` on memory that you don’t allocate using `malloc`. Attempting to deallocate nonallocated memory can result in a crash. Available in Xcode 7 and later.

### Deallocation of a stack variable in C

In the following example, the `value` variable allocates on the stack, and deallocates when the function exits, so calling `free` on it is incorrect:

```
int value = 42;
free(&value); // Error: free called on stack allocated variable
```

#### Solution

Don’t call the `free` function on variables that you allocate on the stack.

## See Also

### Address Sanitizer

Use of deallocated memory

Detects the use of deallocated memory.

Deallocation of deallocated memory

Detects attempts to free deallocated memory.

Use of stack memory after function return

Detects when you access stack variable memory after its declaring function returns.

Use of out-of-scope stack memory

Detects access to variables outside of their declared scope.

Overflow and underflow of buffers

Detects when you access memory outside of a buffer’s boundaries.

Overflow of C++ containers

Detects when you access a C++ container outside its bounds.

