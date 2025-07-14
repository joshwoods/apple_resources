

- Kernel
- Hardware Families
- Mass Storage
- IOMedia
-  getPreferredBlockSize 

# getPreferredBlockSize

``` source
virtual UInt64 getPreferredBlockSize() const; 
```

## Return Value

Natural block size, in bytes.

## Overview

Ask the media object for its natural block size. This information is useful to clients that want to optimize access to the media.

## See Also

### Miscellaneous

copyPhysicalExtent

getAttributes

getBase

getContent

getContentHint

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

