

- Kernel
- Hardware Families
- Mass Storage
- IOBlockStorageDriver
-  instantiateMediaObject 

# instantiateMediaObject

Create an IOMedia object for media.

``` source
virtual IOMedia * instantiateMediaObject(
 UInt64base,
 UInt64byteSize, 
 UInt32blockSize,
 char *mediaName); 
```

## Parameters 

`base`  

Byte number of beginning of active data area of the media. Usually zero.

`byteSize`  

Size of the data area of the media, in bytes.

`blockSize`  

Block size of the media, in bytes.

`mediaName`  

Name of the IOMedia object.

## Return Value

A pointer to the created IOMedia object, or a null on error.

## Overview

This method creates an IOMedia object from the supplied parameters. It is a convenience method to wrap the handful of steps to do the job.

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

