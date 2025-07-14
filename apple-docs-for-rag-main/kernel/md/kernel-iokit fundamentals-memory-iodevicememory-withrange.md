

- Kernel
- IOKit Fundamentals
- Memory
- IODeviceMemory
-  withRange 

# withRange

Constructs an IODeviceMemory instance, describing one physical range.

``` source
static IODeviceMemory * withRange( 
 IOPhysicalAddressaddress, 
 IOPhysicalLengthwithLength ); 
```

## Parameters 

`address`  

The physical address of the first byte in the memory.

`withLength`  

The length of memory.

## Return Value

Returns the created IODeviceMemory on success, to be released by the caller, or zero on failure.

## Overview

This method creates an IODeviceMemory instance for one physical range passed as a physical address and length. It just calls IOMemoryDescriptor::withPhysicalAddress.

## See Also

### Miscellaneous

arrayFromList

Constructs an OSArray of IODeviceMemory instances, each describing one physical range, and a tag value.

withSubRange

Constructs an IODeviceMemory instance, describing a subset of an existing IODeviceMemory range.

