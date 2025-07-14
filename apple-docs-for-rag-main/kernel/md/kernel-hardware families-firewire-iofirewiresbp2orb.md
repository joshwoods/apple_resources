

- Kernel
- Hardware Families
- FireWire
-  IOFireWireSBP2ORB 

Class

# IOFireWireSBP2ORB

Represents an SBP2 normal command ORB. Supplies the APIs for configuring normal command ORBs. This includes setting the command block and writing the page tables for I/O. The ORBs are executed using the submitORB method in IOFireWireSBP2Login.

macOS 10.0+

``` source
class IOFireWireSBP2ORB : IOCommand
```

## Overview

## Topics

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

### Instance Methods

- allocateORB

- allocatePageTable

- allocateResources

- allocateTimer

- calculateTransferSizeLog

- cancelTimer

- completeBufferAddressSpace

- deallocateBufferAddressSpace

- deallocateORB

- deallocatePageTable

- deallocateTimer

- free

- getCommandBufferDescriptor

- getCommandFlags

- getCommandGeneration

- getCommandTimeout

- getFetchAgentWriteRetries

- getFetchAgentWriteRetryInterval

- getFireWireLUN

- getFireWireUnit

- getLogin

- getMaxPayloadSize

- getMetaClass

- getORBAddress

- getRefCon

- getRefCon64

- initWithLogin

- isAppended

- isTimerSet

- orbTimeout

- prepareBufferAddressSpace

- prepareFastStartPacket

- prepareORBForExecution

- release

- releaseCommandBuffers

- removeORB

- sendTimeoutNotification

- setBufferConstraints

- setCommandBlock

- setCommandBlock

- setCommandBuffers

- setCommandBuffersAsRanges

- setCommandBuffersAsRanges64

- setCommandFlags

- setCommandGeneration

- setCommandTimeout

- setFetchAgentWriteRetries

- setFetchAgentWriteRetryInterval

- setIsAppended

- setMaxPayloadSize

- setNextORBAddress

- setRefCon

- setRefCon64

- setToDummy

- startTimer

### Type Methods

+ orbTimeoutStatic

## Relationships

### Inherits From

- IOCommand

## See Also

### Serial Bus Protocol 2

IOFireWireSBP2Login

Supplies the login maintenance and Normal Command ORB execution portions of the API.

IOFireWireSBP2ManagementORB

Supplies non login related management ORBs. Management ORBs can be executed independent of a login, if necessary. Management ORBs are created using the IOFireWireSBP2LUN interface.

FWSBP2FetchAgentWriteCallback

FWSBP2LoginCallback

FWSBP2LoginCompleteParams

FWSBP2LoginCompleteParamsPtr

FWSBP2LoginResponse

FWSBP2LoginResponsePtr

FWSBP2LogoutCallback

FWSBP2LogoutCompleteParams

FWSBP2LogoutCompleteParamsPtr

FWSBP2ManagementCallback

FWSBP2NotifyCallback

FWSBP2NotifyParams

FWSBP2NotifyParamsPtr

FWSBP2ReconnectParams

FWSBP2ReconnectParamsPtr

FWSBP2StatusBlock

FWSBP2StatusCallback

