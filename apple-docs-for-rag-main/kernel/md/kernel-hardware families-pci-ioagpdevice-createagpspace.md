

- Kernel
- Hardware Families
- PCI
- IOAGPDevice
-  createAGPSpace 

# createAGPSpace

Allocates the AGP space, and enables AGP transactions on the primary and secondary.

``` source
virtual IOReturn createAGPSpace(
 IOOptionBitsoptions, 
 IOPhysicalAddress *address, 
 IOPhysicalLength *length ); 
```

## Parameters 

`options`  

No options are currently defined, pass zero.

`address`  

The physical range allocated for the AGP space is passed back to the caller.

`length`  

An in/out parameter - the caller sets the devices maximum AGP addressing and the actual size created is passed back.

## Return Value

Returns an IOReturn code indicating success or failure.

## Overview

This method should be called by the driver for the AGP primary device to set the size of the space and enable AGP transactions. It will destroy any AGP space currently allocated.

## See Also

### Miscellaneous

commitAGPMemory

Makes memory addressable by AGP transactions.

destroyAGPSpace

Destroys the AGP space, and disables AGP transactions on the primary and secondary.

getAGPRangeAllocator

Accessor to obtain the AGP range allocator.

getAGPSpace

Returns the allocated AGP space.

getAGPStatus

Returns the current state of the AGP bus.

releaseAGPMemory

Releases memory addressable by AGP transactions.

