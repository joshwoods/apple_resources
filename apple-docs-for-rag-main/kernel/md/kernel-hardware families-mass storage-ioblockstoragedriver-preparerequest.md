

- Kernel
- Hardware Families
- Mass Storage
- IOBlockStorageDriver
-  prepareRequest 

# prepareRequest

``` source
virtual void prepareRequest(
 UInt64byteStart, 
 IOMemoryDescriptor *buffer, 
 IOStorageAttributes *attributes, 
 IOStorageCompletion *completion); 
```

## Parameters 

`byteStart`  

Starting byte offset for the data transfer.

`buffer`  

Buffer for the data transfer. The size of the buffer implies the size of the data transfer.

`attributes`  

Attributes of the data transfer. See IOStorageAttributes. It is the responsibility of the callee to maintain the information for the duration of the data transfer, as necessary.

`completion`  

Completion routine to call once the data transfer is complete. It is the responsibility of the callee to maintain the information for the duration of the data transfer, as necessary.

## Overview

The prepareRequest method allocates and prepares state for the transfer.

This method is part of a sequence of methods invoked for each read/write request. The first is prepareRequest, which allocates and prepares some context for the transfer; the second is deblockRequest, which aligns the transfer at the media's block boundaries; third is breakUpRequest, which breaks up the transfer into multiple sub-transfers when certain hardware constraints are exceeded; fourth is executeRequest, which implements the actual transfer from the block storage device.

This method's implementation is not typically overridden.

## See Also

### Miscellaneous

acceptNewMedia

React to new media insertion.

addToBytesTransferred

allocateContext

breakUpRequest

checkForMedia

Check if media has newly arrived or disappeared.

constrainByteCount

Constrain the byte count for this IO to device limits.

copyPhysicalExtent

deblockRequest

decommissionMedia

Decommission an existing piece of media that has gone away.

deleteContext

ejectMedia

executeRequest

formatMedia

getDeviceTypeName

Return the desired device name.

getFormatCapacities

getMediaBlockSize

getMediaState

getStatistic

getStatistics

handleClose

handleIsOpen

handleOpen

handleStart

incrementErrors

incrementRetries

initMediaState

Initialize media-related instance variables.

instantiateDesiredMediaObject

Create an IOMedia object for media.

instantiateMediaObject

Create an IOMedia object for media.

isMediaEjectable

isMediaRemovable

isMediaWritable

lockPhysicalExtents

mediaStateHasChanged

React to a new media insertion or a media removal.

read

recordMediaParameters

Obtain media-related parameters on media insertion.

rejectMedia

Reject new media.

requestIdle

Request that the device enter an idle state.

synchronizeCache

unlockPhysicalExtents

unmap

validateNewMedia

Verify that new media is acceptable.

write

