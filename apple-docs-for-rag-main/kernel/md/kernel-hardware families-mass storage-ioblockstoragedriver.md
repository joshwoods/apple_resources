

- Kernel
- Hardware Families
- Mass Storage
-  IOBlockStorageDriver 

Class

# IOBlockStorageDriver

The common base class for generic block storage drivers.

macOS 10.6+

``` source
class IOBlockStorageDriver : IOStorage
```

## Overview

The IOBlockStorageDriver class is the common base class for generic block storage drivers. It matches and communicates via an IOBlockStorageDevice interface, and connects to the remainder of the storage framework via the IOStorage protocol. It extends the IOStorage protocol by implementing the appropriate open and close semantics, deblocking for unaligned transfers, polling for ejectable media, locking and ejection policies, media object creation and tear-down, and statistics gathering and reporting.

Block storage drivers are split into two parts: the generic driver handles all generic device issues, independent of the lower-level transport mechanism (e.g. SCSI, ATA, USB, FireWire). All storage operations at the generic driver level are translated into a series of generic device operations. These operations are passed via the IOBlockStorageDevice nub to a transport driver, which implements the appropriate transport-dependent protocol to execute these operations.

To determine the write-protect state of a device (or media), for example, the generic driver would issue a call to the Transport Driver's reportWriteProtection method. If this were a SCSI device, its transport driver would issue a Mode Sense command to extract the write-protection status bit. The transport driver then reports true or false to the generic driver.

The generic driver therefore has no knowledge of, or involvement with, the actual commands and mechanisms used to communicate with the device. It is expected that the generic driver will rarely, if ever, need to be subclassed to handle device idiosyncrasies; rather, the transport driver should be changed via overrides.

A generic driver could be subclassed to create a different type of generic device. The generic driver IOCDBlockStorageDriver class is a subclass of IOBlockStorageDriver, adding CD functions.

## Topics

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

### Instance Variables

_writeProtected

_removable

_mediaType

_mediaObject

_mediaBlockSize

_maxWriteByteTransfer

_maxReadByteTransfer

_maxBlockNumber

_ejectable

### Instance Methods

- acceptNewMedia

- addToBytesTransferred

- allocateContext

- breakUpRequest

- checkForMedia

- constrainByteCountDeprecated

- copyPhysicalExtent

- deblockRequest

- decommissionMedia

- deleteContext

- didTerminate

- ejectMedia

- executeRequest

- formatMedia

- free

- getDeviceTypeName

- getFormatCapacities

- getMediaBlockSize

- getMediaState

- getMetaClass

- getProvider

- getProvisionStatus

- getStatistic

- getStatistics

- handleClose

- handleIsOpen

- handleOpen

- handleStart

- handleYieldDeprecated

- incrementErrors

- incrementRetries

- init

- initMediaState

- instantiateDesiredMediaObject

- instantiateMediaObject

- isMediaEjectable

- isMediaPollExpensiveDeprecated

- isMediaPollRequiredDeprecated

- isMediaRemovable

- isMediaWritable

- lockMediaDeprecated

- lockPhysicalExtents

- mediaStateHasChanged

- message

- pollMediaDeprecated

- prepareRequest

- read

- recordMediaParameters

- rejectMedia

- requestIdle

- schedulePollerDeprecated

- setPriority

- start

- stop

- synchronize

- systemWillShutdown

- unlockPhysicalExtents

- unmap

- unschedulePollerDeprecated

- validateNewMedia

- write

- yieldDeprecated

### Type Methods

+ breakUpRequestCompletion

+ breakUpRequestExecute

+ deblockRequestCompletion

+ deblockRequestExecute

+ handlePowerEvent

+ prepareRequestCompletion

## Relationships

### Inherits From

- IOStorage

## See Also

### Drivers

IOBDBlockStorageDriver

IODVDBlockStorageDriver

IOCDBlockStorageDriver

IOStorage

The common base class for mass storage objects.

