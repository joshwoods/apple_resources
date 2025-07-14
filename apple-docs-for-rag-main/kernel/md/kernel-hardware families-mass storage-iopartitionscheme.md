

- Kernel
- Hardware Families
- Mass Storage
-  IOPartitionScheme 

Class

# IOPartitionScheme

The common base class for all partition scheme objects.

macOS 10.6+

``` source
class IOPartitionScheme : IOStorage
```

## Overview

The IOPartitionScheme class is the common base class for all partition scheme objects. It extends the IOStorage class by implementing the appropriate open and close semantics for partition objects (standard semantics are to act as a multiplexor for incoming opens, producing one outgoing open with the correct access). It also implements the default read and write semantics, which pass all reads and writes through to the provider media unprocessed. For simple schemes, the default behavior is sufficient. More complex partition schemes such as RAID will want to do extra processing for reads and writes.

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

- attachMediaObjectToDeviceTree

- copyPhysicalExtent

- detachMediaObjectFromDeviceTree

- free

- getMetaClass

- getProvider

- getProvisionStatus

- handleClose

- handleIsOpen

- handleOpen

- init

- juxtaposeMediaObjects

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

IOFilterScheme

The common base class for all filter scheme objects.

