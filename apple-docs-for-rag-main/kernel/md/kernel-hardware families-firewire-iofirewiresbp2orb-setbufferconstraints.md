

- Kernel
- Hardware Families
- FireWire
- IOFireWireSBP2ORB
-  setBufferConstraints 

# setBufferConstraints

Configures page table generation parameters

``` source
IOReturn setBufferConstraints(
 UInt64 maxSegmentSize,
 UInt32 alignment,
 UInt32 options = 0); 
```

## Return Value

May return an error if there is a problem allocating the underlying resources or if buffers are currently attached.

## Overview

Sets the maximums size of any page table segment and the required alignemnt. Double buffering may be used to satisfy these constraints. The only supported option is kFWSBP2ConstraintForceDoubleBuffer which forces a page aligned double buffering of the entire descriptor.

## See Also

### Miscellaneous

allocatePageTable

Allocates memory for the page table.

deallocatePageTable

Frees up memory allocated for the page table.

getCommandBufferDescriptor

Returns the memory descriptor representing the command buffer.

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

