

- Kernel
- Hardware Families
- Mass Storage
- IOBlockStorageDriver
-  getFormatCapacities 

# getFormatCapacities

``` source
virtual UInt32 getFormatCapacities(
 UInt64 *capacities, 
 UInt32capacitiesMaxCount) const; 
```

## Parameters 

`capacities`  

Buffer that will receive the UInt64 capacity values.

`capacitiesMaxCount`  

Maximum number of capacity values that can be held in the buffer.

## Return Value

Actual number of capacity values copied to the buffer, or if no buffer is given, the total number of capacity values available.

## Overview

Ask the driver to report the feasible formatting capacities for the inserted media (in bytes). This routine fills the caller's buffer, up to the maximum count specified if the real number of capacities would overflow the buffer. The return value indicates the actual number of capacities copied to the buffer.

If the capacities buffer is not supplied or if the maximum count is zero, the routine returns the proposed count of capacities instead.

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

