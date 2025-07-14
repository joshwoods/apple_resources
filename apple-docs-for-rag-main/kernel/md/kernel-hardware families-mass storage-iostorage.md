

- Kernel
- Hardware Families
- Mass Storage
-  IOStorage 

Class

# IOStorage

The common base class for mass storage objects.

macOS 10.6+

``` source
class IOStorage : IOService
```

## Overview

The IOStorage class is the common base class for mass storage objects. It is an abstract class that defines the open/close/read/write APIs that need to be implemented in a given subclass. Synchronous versions of the read/write APIs are provided here -- they are coded in such a way as to wrap the asynchronous versions implemented in the subclass.

## Topics

### Miscellaneous

complete

copyPhysicalExtent

handleClose

handleIsOpen

handleOpen

lockPhysicalExtents

open

read()

read()

synchronizeCache

unlockPhysicalExtents

unmap

write()

write()

### Instance Methods

- attach

- copyPhysicalExtent

- discardDeprecated

- getMetaClass

- getProvisionStatus

- handleClose

- handleIsOpen

- handleOpen

- lockPhysicalExtents

- open

- read

- read

- setPriority

- synchronize

- synchronizeCacheDeprecated

- unlockPhysicalExtents

- unmap

- write

- write

### Type Methods

+ complete

## Relationships

### Inherits From

- IOService

## See Also

### Drivers

IOBDBlockStorageDriver

IODVDBlockStorageDriver

IOCDBlockStorageDriver

IOBlockStorageDriver

The common base class for generic block storage drivers.

