

- Kernel
- Hardware Families
- Mass Storage
- IOMedia
-  unmap 

# unmap

``` source
virtual IOReturn unmap(
 IOService *client, 
 IOStorageExtent *extents, 
 UInt32extentsCount, 
 UInt32 options = 0); 
```

## Parameters 

`client`  

Client requesting the operation.

`extents`  

List of extents. See IOStorageExtent. It is legal for the callee to overwrite the contents of this buffer in order to satisfy the request.

`extentsCount`  

Number of extents.

## Return Value

Returns the status of the operation.

## Overview

Delete unused data from the storage object at the specified byte offsets, synchronously.

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

unlockPhysicalExtents

write

