

- Kernel
- Hardware Families
- PCI
- IOAGPDevice
-  commitAGPMemory 

# commitAGPMemory

Makes memory addressable by AGP transactions.

``` source
virtual IOReturn commitAGPMemory(
 IOMemoryDescriptor *memory, 
 IOByteCount agpOffset, 
 IOOptionBits options = 0 ); 
```

## Parameters 

`memory`  

A IOMemoryDescriptor object describing the memory to add to the GART.

`agpOffset`  

An offset into AGP space that the caller has allocated - usually allocated by the AGP range allocator.

`options`  

Pass kIOAGPGartInvalidate if the AGP target should invalidate any GART TLB.

## Return Value

Returns an IOReturn code indicating success or failure.

## Overview

Makes the memory described by the IOMemoryDescriptor object addressable by AGP by entering its pages into the GART array, given an offset into AGP space supplied by the caller (usually allocated by the AGP range allocator). It is the caller's responsibility to prepare non-kernel pageable memory before calling this method, with IOMemoryDescriptor::prepare.

## See Also

### Miscellaneous

createAGPSpace

Allocates the AGP space, and enables AGP transactions on the primary and secondary.

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

