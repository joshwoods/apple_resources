

- Xcode
- Debugging
- Diagnosing memory, thread, and crash issues early
-  Overflow and underflow of buffers 

Article

# Overflow and underflow of buffers

Detects when you access memory outside of a buffer’s boundaries.

## Overview

In Xcode 7 and later, you can use this check to detect when you access memory that’s outside of a buffer’s boundaries. The check reports overflow when accessed memory is beyond the end of the buffer, and underflow when the accessed memory is before the beginning of a buffer. Xcode sanitizes heap and stack buffers, as well as global variables. Buffer overflow and underflow can result in a crash or other unpredictable behavior.

### Global, heap, and stack overflows in C

In the following example, the `global_array`, `heap_buffer`, and `stack_buffer` variables each have valid indexes in the range `[0, 9]`, but the accessed index is `10`, which causes an overflow:

```
int global_array[10] = {0, 1, 2, 3, 4, 5, 6, 7, 8, 9};
void foo() {
    int idx = 10;
    global_array[idx] = 42; // Error: out of bounds access of global variable
    char *heap_buffer = malloc(10);
    heap_buffer[idx] = 'x'; // Error: out of bounds access of heap allocated variable
    char stack_buffer[10];
    stack_buffer[idx] = 'x'; // Error: out of bounds access of stack allocated variable
}
```

#### Solution

Add a bounds check before attempting to access a buffer at a specific index.

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

Overflow of C++ containers

Detects when you access a C++ container outside its bounds.

