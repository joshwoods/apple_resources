

- Kernel
- IOKit Fundamentals
- Memory
-  IOMalloc 

Function

# IOMalloc

Allocates general purpose, wired memory in the kernel map.

macOS 10.0+

``` source
void * IOMalloc(vm_size_t size);
```

## Parameters 

`size`  

Size of the memory requested.

## Return Value

Pointer to the allocated memory, or zero on failure.

## Discussion

This is a general purpose utility to allocate memory in the kernel. There are no alignment guarantees given on the returned memory, and alignment may vary depending on the kernel configuration. This function may block and so should not be called from interrupt level or while a simple lock is held.

## See Also

### Allocation

IOMallocAligned

Allocates wired memory in the kernel map, with an alignment restriction.

IOMallocPageable

Allocates pageable memory in the kernel map.

IOMallocZero

IORangeAllocator

A utility class to manage allocations from a range.

