

- Kernel
- Hardware Families
- Mass Storage
- IOStorage
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

complete

copyPhysicalExtent

handleClose

handleIsOpen

handleOpen

lockPhysicalExtents

open

read()

read()

synchronizeCache

unlockPhysicalExtents

write()

write()

