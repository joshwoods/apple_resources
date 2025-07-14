

- Kernel
- Hardware Families
- Mass Storage
- IOMedia
-  getContent 

# getContent

``` source
virtual const char * getContent() const; 
```

## Return Value

Description of media's contents.

## Overview

Ask the media object for a description of its contents. The description is the same as the hint at the time of the object's creation, but it is possible that the description has been overridden by a client (which has probed the media and identified the content correctly) of the media object. It is more accurate than the hint for this reason. The string is formed in the likeness of Apple's "Apple_HFS" strings or in the likeness of a UUID.

The content description can be overridden by any client that matches onto this media object with a match category of kIOStorageCategory. The media object checks for a kIOMediaContentMaskKey property in the client, and if it finds one, it copies it into kIOMediaContentKey property.

## See Also

### Miscellaneous

copyPhysicalExtent

getAttributes

getBase

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

