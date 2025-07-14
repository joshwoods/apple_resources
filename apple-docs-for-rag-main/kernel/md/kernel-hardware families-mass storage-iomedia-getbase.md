

- Kernel
- Hardware Families
- Mass Storage
- IOMedia
-  getBase 

# getBase

``` source
virtual UInt64 getBase() const; 
```

## Overview

Ask the media object for its byte offset relative to its provider media object below it in the storage hierarchy. Media offset, in bytes.

## See Also

### Miscellaneous

copyPhysicalExtent

getAttributes

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

