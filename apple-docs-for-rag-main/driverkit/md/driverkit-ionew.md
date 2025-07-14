

- DriverKit
-  IONew 

Macro

# IONew

Allocates memory for an array of the specified type.

DriverKitiOSiPadOSmacOS

``` source
#define IONew(type, count)
```

## Parameters 

`type`  

The data type to store in the block of memory. The macro uses the size of this type to determine how much memory to allocate for each array entry.

`count`  

The number of array entries to allocate.

## Return Value

A pointer to the allocated memory block, or `NULL` on failure.

## Discussion

This is a general-purpose utility to allocate memory. There are no alignment guarantees on the returned memory, and alignment may vary depending on the configuration. To allocate memory for use in I/O transfers, create an IOBufferMemoryDescriptor instead.

## See Also

### Allocation

IONewZero

Allocates memory for an array of the specified type and zero-initializes that memory.

IOMalloc

Allocates the specified amount of general-purpose memory.

IOMallocZero

Allocates the specified amount of general-purpose memory and zero-initializes it.

OSTypeAlloc

Allocates memory for a named class.

