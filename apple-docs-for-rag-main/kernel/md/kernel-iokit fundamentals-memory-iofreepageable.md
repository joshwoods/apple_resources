

- Kernel
- IOKit Fundamentals
- Memory
-  IOFreePageable 

Function

# IOFreePageable

Frees memory allocated with IOMallocPageable.

macOS 10.0+

``` source
void IOFreePageable(void *address, vm_size_t size);
```

## Parameters 

`address`  

Virtual address of the allocated memory.

`size`  

Size of the memory allocated.

## Discussion

This function frees memory allocated with IOMallocPageable, it may block and so should not be called from interrupt level or while a simple lock is held.

## See Also

### Deallocation

IOFree

Frees memory allocated with IOMalloc.

IOFreeAligned

Frees memory allocated with IOMallocAligned.

