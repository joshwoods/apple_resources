

- Kernel
- Hardware Families
- Mass Storage
- IOBlockStorageDriver
-  mediaStateHasChanged 

# mediaStateHasChanged

React to a new media insertion or a media removal.

``` source
virtual IOReturn mediaStateHasChanged(
 IOMediaState state); 
```

## Overview

This method is called on a media state change, that is, an arrival or removal. If media has just become available, calls are made to recordMediaParameters and acceptNewMedia. If media has just gone away, a call is made to decommissionMedia, with the forcible parameter set to true. The forcible tear-down is needed to enforce the disappearance of media, regardless of interested clients.

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

