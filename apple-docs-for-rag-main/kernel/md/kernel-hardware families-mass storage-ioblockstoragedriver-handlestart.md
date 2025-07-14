

- Kernel
- Hardware Families
- Mass Storage
- IOBlockStorageDriver
-  handleStart 

# handleStart

``` source
virtual bool handleStart(
 IOService *provider); 
```

## Parameters 

`provider`  

This object's provider.

## Return Value

Returns true on success, false otherwise.

## Overview

Prepare the block storage driver for operation.

This is where a media object needs to be created for fixed media, and optionally for removable media.

Note that this method is called from within the start() routine; if this method returns successfully, it should be prepared to accept any of IOBlockStorageDriver's APIs.

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

