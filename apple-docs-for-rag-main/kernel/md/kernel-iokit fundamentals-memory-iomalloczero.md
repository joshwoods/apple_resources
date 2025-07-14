

- Kernel
- IOKit Fundamentals
- Memory
-  IOMallocZero 

Function

# IOMallocZero

macOS 10.15+

``` source
void * IOMallocZero(vm_size_t size);
```

## See Also

### Allocation

IOMalloc

Allocates general purpose, wired memory in the kernel map.

IOMallocAligned

Allocates wired memory in the kernel map, with an alignment restriction.

IOMallocPageable

Allocates pageable memory in the kernel map.

IORangeAllocator

A utility class to manage allocations from a range.

