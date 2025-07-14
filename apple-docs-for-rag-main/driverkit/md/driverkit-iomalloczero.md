

- DriverKit
-  IOMallocZero 

Function

# IOMallocZero

Allocates the specified amount of general-purpose memory and zero-initializes it.

DriverKitiOSiPadOSmacOS

``` source
void * IOMallocZero(size_t length);
```

## Parameters 

`length`  

The number of bytes to allocate.

## Return Value

A pointer to the allocated memory block, or `NULL` on failure.

## Discussion

This is a general-purpose utility to allocate memory, and initialize that memory to zero. There are no alignment guarantees on the returned memory, and alignment may vary depending on the configuration. To allocate memory for use in I/O transfers, create an IOBufferMemoryDescriptor instead.

## See Also

### Allocation

IONew

Allocates memory for an array of the specified type.

IONewZero

Allocates memory for an array of the specified type and zero-initializes that memory.

IOMalloc

Allocates the specified amount of general-purpose memory.

OSTypeAlloc

Allocates memory for a named class.

