

- Kernel
- Hardware Families
- Mass Storage
- IOBlockStorageDriver
-  constrainByteCount 

# constrainByteCount

Constrain the byte count for this IO to device limits.

``` source
virtual UInt64 constrainByteCount(
 UInt64requestedCount,
 boolisWrite); 
```

## Parameters 

`requestedCount`  

The requested byte count for the next read or write operation.

`isWrite`  

True if the operation will be a write; False if the operation will be a read.

## Overview

This function should be called prior to each read or write operation, so that the driver can constrain the requested byte count, as necessary, to meet current device limits. Such limits could be imposed by the device depending on operating modes, media types, or transport protocol (e.g. ATA, SCSI).

At present, this method is not used.

## See Also

### Miscellaneous

acceptNewMedia

React to new media insertion.

addToBytesTransferred

allocateContext

breakUpRequest

checkForMedia

Check if media has newly arrived or disappeared.

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

prepareRequest

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

