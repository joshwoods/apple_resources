

- Kernel
- Hardware Families
- FireWire
- IOFireWireSBP2ORB
-  getCommandBufferDescriptor 

# getCommandBufferDescriptor

Returns the memory descriptor representing the command buffer.

``` source
virtual IOMemoryDescriptor * getCommandBufferDescriptor(
 void ); 
```

## Return Value

Returns memory descriptor representing mapped data buffers.

## Overview

Returns the IOMemoryDescriptor for the data mapped by setCommandBuffer variants. Works for setCommandBuffersAsRanges too.

## See Also

### Miscellaneous

allocatePageTable

Allocates memory for the page table.

deallocatePageTable

Frees up memory allocated for the page table.

getCommandFlags

Sets configuration flags for the ORB.

getCommandGeneration

Gets the command generation.

getCommandTimeout

Gets the timeout of the ORB.

getLogin

Gets the login associated with this ORB.

getMaxPayloadSize

Gets max payload size for the ORB.

getORBAddress

Returns the FireWire address of this ORB.

getRefCon

Returns the refCon set with setRefCon.

getRefCon64

Returns the 64 bit refCon set with setRefCon64.

release

Primary implementation of the release mechanism.

releaseCommandBuffers

Releases SBP2's reference to the command buffers.

setBufferConstraints

Configures page table generation parameters

setCommandBlock(IOMemoryDescriptor *)

Sets the command block portion of the ORB.

setCommandBlock(void *, UInt32)

Sets the command block portion of the ORB.

setCommandBuffers

Creates a page table from a list of ranges.

setCommandBuffersAsRanges(IOMemoryDescriptor *, UInt32, UInt32)

Creates a page table from a list of ranges.

setCommandBuffersAsRanges(IOVirtualRange *, UInt32, IODirection, task_t, UInt32, UInt32)

Creates a page table from a list of ranges.

setCommandBuffersAsRanges64

Creates a page table from a list of 64 bit ranges.

setCommandFlags

Sets configuration flags for the ORB.

setCommandGeneration

Sets the command generation.

setCommandTimeout

Sets the timeout of the ORB.

setMaxPayloadSize

Sets max payload size for the ORB.

setRefCon

Sets the ORB refCon.

setRefCon64

Sets the ORB refCon as a 64 bit value.

