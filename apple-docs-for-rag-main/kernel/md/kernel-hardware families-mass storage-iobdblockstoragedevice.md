

- Kernel
- Hardware Families
- Mass Storage
-  IOBDBlockStorageDevice 

Class

# IOBDBlockStorageDevice

The IOBDBlockStorageDevice class is a generic BD block storage device abstraction.

macOS 10.6+

``` source
class IOBDBlockStorageDevice : IODVDBlockStorageDevice
```

## Overview

This class is the protocol for generic BD functionality, independent of the physical connection protocol (e.g. SCSI, ATA, USB).

The APIs are the union of CD APIs, DVD APIs, and all necessary new low-level BD APIs.

A subclass implements relay methods that translate our requests into calls to a protocol- and device-specific provider.

## Topics

### Miscellaneous

init

readDiscStructure

splitTrack

### Instance Methods

- getMetaClass

- init

- readDiscStructure

- splitTrack

## Relationships

### Inherits From

- IODVDBlockStorageDevice

## See Also

### Interfaces

IODVDServices

IODVDBlockStorageDevice

The IODVDBlockStorageDevice class is a generic DVD block storage device abstraction.

IOCompactDiscServices

IOBDMediaBSDClient

IOMediaBSDClient

