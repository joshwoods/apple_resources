

- Kernel
- Hardware Families
- Mass Storage
-  IOCDMedia 

Class

# IOCDMedia

The IOCDMedia class is a random-access disk device abstraction for CDs.

macOS 10.6+

``` source
class IOCDMedia : IOMedia
```

## Overview

The IOCDMedia class is a random-access disk device abstraction for CDs. It extends the IOMedia class by implementing special CD APIs, such as readCD, and publishing the TOC as a property of the IOCDMedia object.

## Topics

### Miscellaneous

getSpeed

getTOC

read

readCD()

readCD()

readDiscInfo

readISRC

readMCN

readTOC

readTrackInfo

setSpeed

### Instance Methods

- getMetaClass

- getProvider

- getSpeed

- getTOC

- matchPropertyTable

- read

- readCD

- readCD

- readDiscInfo

- readISRC

- readMCN

- readTOC

- readTrackInfo

- setSpeed

- write

- writeCD

- writeCD

## Relationships

### Inherits From

- IOMedia

## See Also

### Data Storage

IOBDMedia

The IOBDMedia class is a random-access disk device abstraction for BDs.

IOMedia

A random-access disk device abstraction.

IOCDMediaBSDClient

IOCDPartitionScheme

IODVDMedia

The IODVDMedia class is a random-access disk device abstraction for DVDs.

IODVDMediaBSDClient

