

- Kernel
- Hardware Families
- Mass Storage
-  IOBlockStorageDevice 

Class

# IOBlockStorageDevice

A generic block storage device abstraction.

macOS 10.6+

``` source
class IOBlockStorageDevice : IOService
```

## Overview

The IOBlockStorageDevice class exports the generic block storage protocol, independent of the physical connection protocol (e.g. SCSI, ATA, USB), forwarding all requests to its provider (the Transport Driver). Though the nub does no actual processing of requests, it is necessary in a C++ environment. The Transport Driver can be of any type, as long as it inherits from IOService. Because Transport Drivers needn't derive from a type known to IOBlockStorageDriver, it isn't possible for IOBlockStorageDriver to include the appropriate header file to allow direct communication with the Transport Driver. Thus we achieve polymorphism by having the Transport Driver instantiate a subclass of IOBlockStorageDevice. A typical implementation for a concrete subclass of IOBlockStorageDevice simply relays all methods to its provider (the Transport Driver), which implements the protocol- and device-specific behavior.

All pure-virtual functions must be implemented by the Transport Driver, which is responsible for instantiating the Nub.

## Topics

### Miscellaneous

doAsyncReadWrite

Start an asynchronous read or write operation.

doEjectMedia

Eject the media.

doFormatMedia

Format the media to the specified byte capacity.

doGetFormatCapacities

Return the allowable formatting byte capacities.

doSynchronizeCache

Force data blocks in the hardware's buffer to be flushed to the media.

doUnmap

Delete unused data blocks from the media.

getAdditionalDeviceInfoString

Return additional informational string for the device.

getProductString

Return Product Name string for the device.

getRevisionString

Return Product Revision string for the device.

getVendorString

Return Vendor Name string for the device.

getWriteCacheState

Reports the current write cache state of the device.

init

reportBlockSize

Report the block size for the device, in bytes.

reportEjectability

Report if the media is ejectable under software control.

reportMaxValidBlock

Report the highest valid block for the device.

reportMediaState

Report the device's media state.

reportRemovability

Report whether the media is removable or not.

reportWriteProtection

Report whether the media is write-protected or not.

requestIdle

Request that the device enter an idle state.

setWriteCacheState

Sets the write cache state of the device.

### Instance Methods

- doAsyncReadWrite

- doDiscardDeprecated

- doEjectMedia

- doFormatMedia

- doGetFormatCapacities

- doGetProvisionStatus

- doLockUnlockMediaDeprecated

- doSetPriority

- doSynchronize

- doSynchronizeCacheDeprecated

- doUnmap

- getAdditionalDeviceInfoString

- getMetaClass

- getProductString

- getProperty

- getRevisionString

- getVendorString

- getWriteCacheState

- init

- reportBlockSize

- reportEjectability

- reportLockabilityDeprecated

- reportMaxValidBlock

- reportMediaState

- reportPollRequirementsDeprecated

- reportRemovability

- reportWriteProtection

- requestIdle

- setProperties

- setWriteCacheState

## Relationships

### Inherits From

- IOService

## See Also

### Devices

IOBlockStorageServices

IOCDBlockStorageDevice

The IOCDBlockStorageDevice class is a generic CD block storage device abstraction.

IOBDServices

