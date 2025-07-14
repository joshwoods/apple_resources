

- Kernel
- Hardware Families
- PCI
- IOAGPDevice
-  getAGPRangeAllocator 

# getAGPRangeAllocator

Accessor to obtain the AGP range allocator.

``` source
virtual IORangeAllocator * getAGPRangeAllocator(
 void ); 
```

## Return Value

Returns a pointer to the range allocator for the AGP space.

## Overview

To allocate ranges in AGP space, obtain a range allocator for the space with this method. It is retained while the space is created (until destroyAGPSpace is called) and should not be released by the caller.

## See Also

### Miscellaneous

commitAGPMemory

Makes memory addressable by AGP transactions.

createAGPSpace

Allocates the AGP space, and enables AGP transactions on the primary and secondary.

destroyAGPSpace

Destroys the AGP space, and disables AGP transactions on the primary and secondary.

getAGPSpace

Returns the allocated AGP space.

getAGPStatus

Returns the current state of the AGP bus.

releaseAGPMemory

Releases memory addressable by AGP transactions.

