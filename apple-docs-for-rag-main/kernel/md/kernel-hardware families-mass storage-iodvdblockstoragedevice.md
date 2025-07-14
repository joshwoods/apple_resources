

- Kernel
- Hardware Families
- Mass Storage
-  IODVDBlockStorageDevice 

Class

# IODVDBlockStorageDevice

The IODVDBlockStorageDevice class is a generic DVD block storage device abstraction.

macOS 10.6+

``` source
class IODVDBlockStorageDevice : IOCDBlockStorageDevice
```

## Overview

This class is the protocol for generic DVD functionality, independent of the physical connection protocol (e.g. SCSI, ATA, USB).

The APIs are the union of CD APIs and all necessary new low-level DVD APIs.

A subclass implements relay methods that translate our requests into calls to a protocol- and device-specific provider.

## Topics

### Instance Methods

- getMetaClass

- init

- readDVDStructure

- reportKeyDeprecated

- reportKey

- sendKey

## Relationships

### Inherits From

- IOCDBlockStorageDevice

## See Also

### Interfaces

IODVDServices

IOBDBlockStorageDevice

The IOBDBlockStorageDevice class is a generic BD block storage device abstraction.

IOCompactDiscServices

IOBDMediaBSDClient

IOMediaBSDClient

