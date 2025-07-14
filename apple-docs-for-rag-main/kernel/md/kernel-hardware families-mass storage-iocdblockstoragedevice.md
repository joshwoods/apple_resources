

- Kernel
- Hardware Families
- Mass Storage
-  IOCDBlockStorageDevice 

Class

# IOCDBlockStorageDevice

The IOCDBlockStorageDevice class is a generic CD block storage device abstraction.

macOS 10.6+

``` source
class IOCDBlockStorageDevice : IOBlockStorageDevice
```

## Overview

This class is the protocol for generic CD functionality, independent of the physical connection protocol (e.g. SCSI, ATA, USB).

The APIs are the union of CD (block storage) data APIs and all necessary low-level CD APIs.

A subclass implements relay methods that translate our requests into calls to a protocol- and device-specific provider.

## Topics

### Instance Methods

- doAsyncReadCD

- getMediaType

- getMetaClass

- getSpeed

- init

- readDiscInfo

- readISRC

- readMCN

- readTOC

- readTOC

- readTrackInfo

- setSpeed

## Relationships

### Inherits From

- IOBlockStorageDevice

## See Also

### Devices

IOBlockStorageServices

IOBDServices

IOBlockStorageDevice

A generic block storage device abstraction.

