

- Kernel
- Hardware Families
- PCI
- IOAGPDevice
-  getAGPStatus 

# getAGPStatus

Returns the current state of the AGP bus.

``` source
virtual IOOptionBits getAGPStatus(
 IOOptionBits which = which ); 
```

## Parameters 

`which`  

Type of status - only kIOAGPDefaultStatus is currently valid.

## Return Value

Returns mask of status bits for the AGP bus.

## Overview

Returns state bits for the AGP bus. Only one type of status is currently defined.

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

getAGPSpace

Returns the allocated AGP space.

releaseAGPMemory

Releases memory addressable by AGP transactions.

