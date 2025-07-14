

- Kernel
- Hardware Families
- Mass Storage
- IOMedia
-  getAttributes 

# getAttributes

``` source
virtual IOMediaAttributeMask getAttributes() const; 
```

## Return Value

Media attributes, such as ejectability and removability. See IOMediaAttributeMask.

## Overview

Ask the media object for its attributes.

## See Also

### Miscellaneous

copyPhysicalExtent

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

