

- Kernel
- Hardware Families
- PCI
- IOAGPDevice
-  getAGPSpace 

# getAGPSpace

Returns the allocated AGP space.

``` source
virtual IOReturn getAGPSpace(
 IOPhysicalAddress *address, 
 IOPhysicalLength *length ); 
```

## Parameters 

`address`  

The physical range allocated for the AGP space is passed back to the caller. Zero may be passed if the address is not needed by the caller.

`length`  

The size of the the AGP space created is passed back. Zero may be passed if the length is not needed by the caller.

## Return Value

Returns an IOReturn code indicating success or failure.

## Overview

This method can be called by the driver for the AGP primary device to retrieve the physical address and size of the space created with createAGPSpace.

## See Also

### Miscellaneous

commitAGPMemory

Makes memory addressable by AGP transactions.

createAGPSpace

Allocates the AGP space, and enables AGP transactions on the primary and secondary.

destroyAGPSpace

Destroys the AGP space, and disables AGP transactions on the primary and secondary.

getAGPRangeAllocator

Accessor to obtain the AGP range allocator.

getAGPStatus

Returns the current state of the AGP bus.

releaseAGPMemory

Releases memory addressable by AGP transactions.

