

- Kernel
- Hardware Families
- Mass Storage
-  IOFilterScheme 

Class

# IOFilterScheme

The common base class for all filter scheme objects.

macOS 10.6+

``` source
class IOFilterScheme : IOStorage
```

## Overview

The IOFilterScheme class is the common base class for all filter scheme objects. It extends the IOStorage class by implementing the appropriate open and close semantics for filter objects (standard semantics are act as a relay for incoming opens, producing one outgoing open for each incoming open). It also implements the default read and write semantics, which pass all reads and writes through to the provider media unprocessed. For simple schemes, the default behavior is sufficient. More complex filter schemes such as RAID will want to do extra processing for reads and writes.

## Topics

### Miscellaneous

copyPhysicalExtent

handleClose

handleIsOpen

handleOpen

lockPhysicalExtents

read

synchronizeCache

unlockPhysicalExtents

unmap

write

### Instance Methods

- copyPhysicalExtent

- getMetaClass

- getProvider

- getProvisionStatus

- handleClose

- handleIsOpen

- handleOpen

- lockPhysicalExtents

- read

- setPriority

- synchronize

- unlockPhysicalExtents

- unmap

- write

## Relationships

### Inherits From

- IOStorage

## See Also

### Schemes

IOAppleLabelScheme

IOApplePartitionScheme

IOFDiskPartitionScheme

IOGUIDPartitionScheme

IOPartitionScheme

The common base class for all partition scheme objects.

