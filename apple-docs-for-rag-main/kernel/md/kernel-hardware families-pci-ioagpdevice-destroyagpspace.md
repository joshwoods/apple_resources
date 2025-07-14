

- Kernel
- Hardware Families
- PCI
- IOAGPDevice
-  destroyAGPSpace 

# destroyAGPSpace

Destroys the AGP space, and disables AGP transactions on the primary and secondary.

``` source
virtual IOReturn destroyAGPSpace(
 void ); 
```

## Overview

This method should be called by the driver to shutdown AGP transactions and release resources.

## See Also

### Miscellaneous

commitAGPMemory

Makes memory addressable by AGP transactions.

createAGPSpace

Allocates the AGP space, and enables AGP transactions on the primary and secondary.

getAGPRangeAllocator

Accessor to obtain the AGP range allocator.

getAGPSpace

Returns the allocated AGP space.

getAGPStatus

Returns the current state of the AGP bus.

releaseAGPMemory

Releases memory addressable by AGP transactions.

