

- Kernel
- Hardware Families
- Mass Storage
- IOMedia
-  synchronizeCache 

# synchronizeCache

``` source
virtual IOReturn synchronizeCache(
 IOService *client); 
```

## Parameters 

`client`  

Client requesting the cache synchronization.

## Return Value

Returns the status of the cache synchronization.

## Overview

Flush the cached data in the storage object, if any, synchronously.

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

unlockPhysicalExtents

unmap

write

