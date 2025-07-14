

- Kernel
- Hardware Families
- FireWire
- IOFireWireSBP2ORB
-  setCommandFlags 

# setCommandFlags

Sets configuration flags for the ORB.

``` source
virtual void setCommandFlags(
 UInt32flags ); 
```

## Parameters 

`flags`  

The flags to be set.

## Overview

Sets the configuration flags for the ORB. These can be any of the following:

kFWSBP2CommandCompleteNotify - Set the notify bit as specified in SBP2 standard. Set to receive completion/timeout notification on this ORB. You almost always want to set this.

kFWSBP2CommandTransferDataFromTarget - Transfer direction as specified in SBP2 standard. Set if data is to be written by the device into the host's memory.

kFWSBP2CommandImmediate - Immediate Append. ORB address will be written to fetch agent and not chained. It is only legal to have one immediate ORB in progress at a time.

kFWSBP2CommandNormalORB - ORB format 0 - Format specified by SBP2 standard. Set this for most ORBs.

kFWSBP2CommandReservedORB - ORB format 1 - Format reserved by SBP2 standard for future standardization.

kFWSBP2CommandVendorORB - ORB format 2 - Format specified by SBP2 standard for vendor dependent ORBs.

kFWSBP2CommandDummyORB - ORB format 3 - Format specified by SBP2 standard for placeholder ORBs.

kFWSBP2CommandCheckGeneration - If set upon submitORB, the ORB will only be appended if generation set with setCommandGeneration() matches the current generation. Pretty much all SBP2 drivers need sophisticated logic to track login state, so this is generally not used.

kFWSBP2CommandFixedSize - Do not allocate more memory for page table if needed. If there is not enough space in the currently allocated page table, the setCommandBuffers call will fail. This is important to set if your device is the backing store, as we don't want to cause memory allocations on the paging path.

kFWSBP2CommandVirtualORBs - Normally ORBs are backed by physical address spaces. Setting this flag makes this ORB backed by a pseudo address space. This can make ORBs easier to see in a bus trace. Virtual ORBs will have an address in the form of ffcX.XXXX.0000.0000. Pseudo address space backed ORBs are slower, so you won't want to set for deployment builds.

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

setCommandBuffersAsRanges64

Creates a page table from a list of 64 bit ranges.

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

