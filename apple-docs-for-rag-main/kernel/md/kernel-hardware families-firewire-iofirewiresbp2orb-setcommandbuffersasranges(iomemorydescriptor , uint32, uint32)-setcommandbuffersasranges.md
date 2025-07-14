

- Kernel
- Hardware Families
- FireWire
- IOFireWireSBP2ORB
-  setCommandBuffersAsRanges(IOMemoryDescriptor \*, UInt32, UInt32) 

# setCommandBuffersAsRanges(IOMemoryDescriptor \*, UInt32, UInt32)

Creates a page table from a list of ranges.

``` source
virtual IOReturn setCommandBuffers(
 IOMemoryDescriptor *memoryDescriptor,
 UInt32 offset = 0, 
 UInt32 length = 0 ); 
```

## Parameters 

`memoryDescriptor`  

IOMemoryDescriptor describe ranges to be written to a page table.

`offset`  

Offset in bytes into data to begin writing table at.

`length`  

Number of bytes of data to map from offset.

## Return Value

Returns KIOReturnSuccess if the page table was written successfully.

## Overview

Creates a page table with the given parameters. Any addresses mapped by this method must remain valid until setCommandBuffers is called again or releaseCommandBuffers is called. The SBP2 services do not release references to the command buffers just because the command has completed.

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

setBufferConstraints

Configures page table generation parameters

setCommandBlock(IOMemoryDescriptor *)

Sets the command block portion of the ORB.

setCommandBlock(void *, UInt32)

Sets the command block portion of the ORB.

setCommandBuffers

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

