

- Kernel
- Hardware Families
- Mass Storage
- IOMedia
-  unlockPhysicalExtents 

# unlockPhysicalExtents

``` source
virtual void unlockPhysicalExtents(
 IOService *client); 
```

## Parameters 

`client`  

Client requesting the operation.

## Overview

Unlock the contents of the storage object for relocation again. This call must balance a successful call to lockPhysicalExtents().

## See Also

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

unmap

write

