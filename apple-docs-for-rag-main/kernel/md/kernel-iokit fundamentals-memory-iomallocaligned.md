

- Kernel
- IOKit Fundamentals
- Memory
-  IOMallocAligned 

Function

# IOMallocAligned

Allocates wired memory in the kernel map, with an alignment restriction.

macOS 10.0+

``` source
void * IOMallocAligned(vm_size_t size, vm_offset_t alignment);
```

## Parameters 

`size`  

Size of the memory requested.

`alignment`  

Byte count of the alignment for the memory. For example, pass 256 to get memory allocated at an address with bit 0-7 zero.

## Return Value

Pointer to the allocated memory, or zero on failure.

## Discussion

This is a utility to allocate memory in the kernel, with an alignment restriction which is specified as a byte count. This function may block and so should not be called from interrupt level or while a simple lock is held.

## See Also

### Allocation

IOMalloc

Allocates general purpose, wired memory in the kernel map.

IOMallocPageable

Allocates pageable memory in the kernel map.

IOMallocZero

IORangeAllocator

A utility class to manage allocations from a range.

