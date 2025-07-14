

- Kernel
- Deprecated Symbols
-  IOFreeContiguous Deprecated

Function

# IOFreeContiguous

Deprecated - use IOBufferMemoryDescriptor. Frees memory allocated with IOMallocContiguous.

macOS 10.0–10.6Deprecated

``` source
void IOFreeContiguous(void *address, vm_size_t size);
```

## Parameters 

`address`  

Virtual address of the allocated memory.

`size`  

Size of the memory allocated.

## Discussion

This function frees memory allocated with IOMallocContiguous, it may block and so should not be called from interrupt level or while a simple lock is held.

