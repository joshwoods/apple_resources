

- DriverKit
-  OSTypeAlloc 

Macro

# OSTypeAlloc

Allocates memory for a named class.

DriverKitiOSiPadOSmacOS

``` source
#define OSTypeAlloc(type)
```

## Parameters 

`type`  

The name of the desired class as a raw token, not as a string or macro.

## Return Value

A pointer to the allocated memory block, or `NULL` on failure.

## Discussion

This is a general-purpose utility to allocate memory for DriverKit objects. Consider using object-specific creation methods instead. To allocate memory for use in I/O transfers, create an IOBufferMemoryDescriptor instead.

## See Also

### Allocation

IONew

Allocates memory for an array of the specified type.

IONewZero

Allocates memory for an array of the specified type and zero-initializes that memory.

IOMalloc

Allocates the specified amount of general-purpose memory.

IOMallocZero

Allocates the specified amount of general-purpose memory and zero-initializes it.

