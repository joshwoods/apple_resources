

- Kernel
- IOKit Fundamentals
- Memory
-  IOFree 

Function

# IOFree

Frees memory allocated with IOMalloc.

macOS 10.0+

``` source
void IOFree(void *address, vm_size_t size);
```

## Parameters 

`address`  

Pointer to the allocated memory. Must be identical to result @of a prior IOMalloc.

`size`  

Size of the memory allocated. Must be identical to size of @the corresponding IOMalloc

## Discussion

This function frees memory allocated with IOMalloc, it may block and so should not be called from interrupt level or while a simple lock is held.

## See Also

### Deallocation

IOFreeAligned

Frees memory allocated with IOMallocAligned.

IOFreePageable

Frees memory allocated with IOMallocPageable.

