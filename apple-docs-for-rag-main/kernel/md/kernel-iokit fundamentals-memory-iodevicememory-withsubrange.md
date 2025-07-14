

- Kernel
- IOKit Fundamentals
- Memory
- IODeviceMemory
-  withSubRange 

# withSubRange

Constructs an IODeviceMemory instance, describing a subset of an existing IODeviceMemory range.

``` source
static IODeviceMemory * withSubRange( 
 IODeviceMemory *of, 
 IOPhysicalAddressoffset, 
 IOPhysicalLengthlength ); 
```

## Parameters 

`of`  

The parent IODeviceMemory of which a subrange is to be used for the new descriptor, which will be retained by the subrange IODeviceMemory.

`offset`  

A byte offset into the parent's memory.

`length`  

The length of the subrange.

## Return Value

Returns the created IODeviceMemory on success, to be released by the caller, or zero on failure.

## Overview

This method creates an IODeviceMemory instance for a subset of an existing IODeviceMemory range, passed as a physical address offset and length. It just calls IOMemoryDescriptor::withSubRange.

## See Also

### Miscellaneous

arrayFromList

Constructs an OSArray of IODeviceMemory instances, each describing one physical range, and a tag value.

withRange

Constructs an IODeviceMemory instance, describing one physical range.

