

- Kernel
- IOKit Fundamentals
- Memory
-  IOFreeAligned 

Function

# IOFreeAligned

Frees memory allocated with IOMallocAligned.

macOS 10.0+

``` source
void IOFreeAligned(void *address, vm_size_t size);
```

## Parameters 

`address`  

Pointer to the allocated memory.

`size`  

Size of the memory allocated.

## Discussion

This function frees memory allocated with IOMallocAligned, it may block and so should not be called from interrupt level or while a simple lock is held.

## See Also

### Deallocation

IOFree

Frees memory allocated with IOMalloc.

IOFreePageable

Frees memory allocated with IOMallocPageable.

