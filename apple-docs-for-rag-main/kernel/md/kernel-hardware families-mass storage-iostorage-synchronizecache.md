

- Kernel
- Hardware Families
- Mass Storage
- IOStorage
-  synchronizeCache 

# synchronizeCache

``` source
virtual IOReturn synchronizeCache(
 IOService *client) = 0; 
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

complete

copyPhysicalExtent

handleClose

handleIsOpen

handleOpen

lockPhysicalExtents

open

read()

read()

unlockPhysicalExtents

unmap

write()

write()

