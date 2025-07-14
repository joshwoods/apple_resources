

- Kernel
- Hardware Families
- Mass Storage
-  IOMedia 

Class

# IOMedia

A random-access disk device abstraction.

macOS 10.6+

``` source
class IOMedia : IOStorage
```

## Overview

The IOMedia class is a random-access disk device abstraction. It provides a consistent interface for both real and virtual disk devices, for subdivisions of disks such as partitions, for supersets of disks such as RAID volumes, and so on. It extends the IOStorage class by implementing the appropriate open, close, read, write, and matching semantics for media objects. The properties it has reflect the properties of real disk devices, such as ejectability and writability.

The read and write interfaces support byte-level access to the storage space, with the appropriate deblocking handled by the block storage driver, however, a typical client will want to get the natural block size in order to optimize access to the real disk device. A read or write is accepted so long as the client's access is valid, the media is formatted and the transfer is within the bounds of the media. An optional non-zero base (offset) is then applied before the read or write is passed to provider object.

## Topics

### Miscellaneous

copyPhysicalExtent

getAttributes

getBase

getContent

getContentHint

getPreferredBlockSize

getSize

handleClose

handleIsOpen

handleOpen

init

isEjectable

isFormatted

isWhole

isWritable

lockPhysicalExtents

read

synchronizeCache

unlockPhysicalExtents

unmap

write

### Instance Methods

- attachToChild

- copyPhysicalExtent

- detachFromChild

- free

- getAttributes

- getBase

- getContent

- getContentHint

- getMetaClass

- getPreferredBlockSize

- getProvider

- getProvisionStatus

- getSize

- handleClose

- handleIsOpen

- handleOpen

- init

- isEjectable

- isFormatted

- isWhole

- isWritable

- lockPhysicalExtents

- matchPropertyTable

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

### Data Storage

IOCDMedia

The IOCDMedia class is a random-access disk device abstraction for CDs.

IOBDMedia

The IOBDMedia class is a random-access disk device abstraction for BDs.

IOCDMediaBSDClient

IOCDPartitionScheme

IODVDMedia

The IODVDMedia class is a random-access disk device abstraction for DVDs.

IODVDMediaBSDClient

