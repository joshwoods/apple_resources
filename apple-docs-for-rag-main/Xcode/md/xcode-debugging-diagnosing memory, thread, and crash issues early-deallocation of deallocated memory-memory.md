

- Xcode
- Debugging
- Diagnosing memory, thread, and crash issues early
-  Deallocation of deallocated memory 

Article

# Deallocation of deallocated memory

Detects attempts to free deallocated memory.

## Overview

Use this check to detect when you call `free` on deallocated memory, commonly referred to as a *double free* error. Attempting to deallocate memory more than once can result in a crash or other unpredictable behavior. Available in Xcode 7 and later.

### Deallocation of freed memory in C

In the following example, the code deallocates the `p_int` variable after the call to free its memory:

```
```

#### Solution

Ensure that you call the `free` function just once for memory you allocate.

## See Also

### Address Sanitizer

Use of deallocated memory

Detects the use of deallocated memory.

Deallocation of nonallocated memory

Detects attempts to free nonallocated memory.

Use of stack memory after function return

Detects when you access stack variable memory after its declaring function returns.

Use of out-of-scope stack memory

Detects access to variables outside of their declared scope.

Overflow and underflow of buffers

Detects when you access memory outside of a buffer’s boundaries.

Overflow of C++ containers

Detects when you access a C++ container outside its bounds.

