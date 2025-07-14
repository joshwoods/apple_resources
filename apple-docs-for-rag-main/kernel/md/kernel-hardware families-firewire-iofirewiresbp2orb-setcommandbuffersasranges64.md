

- Kernel
- Hardware Families
- FireWire
- IOFireWireSBP2ORB
-  setCommandBuffersAsRanges64 

# setCommandBuffersAsRanges64

Creates a page table from a list of 64 bit ranges.

``` source
IOReturn setCommandBuffersAsRanges64(
 IOAddressRange *ranges, 
 uint64_t withCount, 
 IODirection withDirection, 
 task_t withTask, 
 uint64_t offset = 0, 
 uint64_t length = 0); 
```

## Parameters 

`ranges`  

An array of ranges representing the data to be transfered.

`withCount`  

The number of ranges in the ranges array.

`withDirection`  

An IODirection indicating the direction of data transfer.

`withTask`  

The task that these adressses reside in.

`offset`  

Offset in bytes into data to begin writing table at.

`length`  

Number of bytes of data to map from offset.

## Return Value

Returns KIOReturnSuccess if the page table was written successfully.

## Overview

Creates a page table with the given parameters. Any addresses mapped by this method must remain valid until setCommandBuffers is called again or releaseCommandBuffers is called. The SBP2 services do not release references to the command buffers just because the command has completed. This is a 64 bit compatible version of setCommandBuffersAsRanges.

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

setCommandBuffersAsRanges(IOMemoryDescriptor *, UInt32, UInt32)

Creates a page table from a list of ranges.

setCommandBuffersAsRanges(IOVirtualRange *, UInt32, IODirection, task_t, UInt32, UInt32)

Creates a page table from a list of ranges.

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

