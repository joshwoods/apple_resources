

- Kernel
- Hardware Families
- Mass Storage
- IOMedia
-  getContentHint 

# getContentHint

``` source
virtual const char * getContentHint() const; 
```

## Return Value

Hint of media's contents.

## Overview

Ask the media object for a hint of its contents. The hint is set at the time of the object's creation, should the creator have a clue as to what it may contain. The hint string does not change for the lifetime of the object and is also formed in the likeness of Apple's "Apple_HFS" strings or in the likeness of a UUID.

## See Also

### Miscellaneous

copyPhysicalExtent

getAttributes

getBase

getContent

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

