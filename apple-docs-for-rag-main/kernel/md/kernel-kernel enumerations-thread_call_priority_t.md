

- Kernel
- Kernel Enumerations
-  thread_call_priority_t 

Enumeration

# thread_call_priority_t

macOS 10.8+

``` source
typedef enum thread_call_priority_t : unsigned int {
    ...
} thread_call_priority_t;
```

## Overview

Thread call priorities should not be assumed to have any specific numerical value; they should be interpreted as importances or roles for work items, priorities for which will be reasonably managed by the subsystem.

## Topics

### Constants

THREAD_CALL_PRIORITY_HIGH

THREAD_CALL_PRIORITY_KERNEL

THREAD_CALL_PRIORITY_USER

THREAD_CALL_PRIORITY_LOW

THREAD_CALL_PRIORITY_KERNEL_HIGH

