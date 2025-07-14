

- Xcode
- Debugging
- Diagnosing memory, thread, and crash issues early
-  Overflow of C++ containers 

Article

# Overflow of C++ containers

Detects when you access a C++ container outside its bounds.

## Overview

Use this check to detect when you access a libc++ container beyond the region `[container.begin(), container.end()]`, even when the accessed memory is in a heap-allocated buffer the container uses internally. Available in Xcode 7 and later.

Note

This check is in a disabled state by default because it requires building all statically linked libraries using `std::vector` with an enabled Address Sanitizer. To enable this check, choose the Yes option for the Enable C++ Container Overflow Checks setting.

### Vector overflow in C++

In the following example, the `vector` variable has valid indexes in the range `[0,2]`, but the accessed index is `3`, which causes an overflow:

```
std::vector vector;
vector.push_back(0);
vector.push_back(1);
vector.push_back(2);
auto *pointer = &vector[0];
return pointer[3]; // Error: out of bounds access for vector
```

#### Solution

Add a bounds check before attempting to access a container at a specific index.

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

Use of out-of-scope stack memory

Detects access to variables outside of their declared scope.

Overflow and underflow of buffers

Detects when you access memory outside of a buffer’s boundaries.

