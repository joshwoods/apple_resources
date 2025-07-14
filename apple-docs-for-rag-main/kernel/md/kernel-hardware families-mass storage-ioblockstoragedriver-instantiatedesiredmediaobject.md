

- Kernel
- Hardware Families
- Mass Storage
- IOBlockStorageDriver
-  instantiateDesiredMediaObject 

# instantiateDesiredMediaObject

Create an IOMedia object for media.

``` source
virtual IOMedia * instantiateDesiredMediaObject(
 void); 
```

## Overview

This method creates the exact type of IOMedia object desired. It is called by instantiateMediaObject. A subclass may override this one-line method to change the type of media object actually instantiated.

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

