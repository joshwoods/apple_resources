

- DriverKit
-  IOFree 

Function

# IOFree

Frees a memory block that contains general-purpose memory.

DriverKitiOSiPadOSmacOS

``` source
void IOFree(void * address, size_t length);
```

## Parameters 

`address`  

The pointer to the memory block to free. The memory block must be one that you previously allocated with IOMalloc or IOMallocZero.

`length`  

The size of the memory block, which must match the block’s original allocation size.

## Discussion

Use this macro to free memory that you allocated with IOMalloc or IOMallocZero.

## See Also

### Deallocation

IODelete

Frees the memory associated with a valid, typed array.

IOSafeDeleteNULL

Frees the memory associated with a typed array.

OSSafeReleaseNULL

Frees memory that you allocated for a named class.

