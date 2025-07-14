

- Kernel
- IOKit Fundamentals
- Memory
-  IOMallocPageable 

Function

# IOMallocPageable

Allocates pageable memory in the kernel map.

macOS 10.0+

``` source
void * IOMallocPageable(vm_size_t size, vm_size_t alignment);
```

## Parameters 

`size`  

Size of the memory requested.

`alignment`  

Byte count of the alignment for the memory. For example, pass 256 to get memory allocated at an address with bits 0-7 zero.

## Return Value

Pointer to the allocated memory, or zero on failure.

## Discussion

This is a utility to allocate pageable memory in the kernel. This function may block and so should not be called from interrupt level or while a simple lock is held.

## See Also

### Allocation

IOMalloc

Allocates general purpose, wired memory in the kernel map.

IOMallocAligned

Allocates wired memory in the kernel map, with an alignment restriction.

IOMallocZero

IORangeAllocator

A utility class to manage allocations from a range.

