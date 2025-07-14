

- Kernel
- Hardware Families
- Mass Storage
- IOPartitionScheme
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

handleClose

handleIsOpen

handleOpen

lockPhysicalExtents

read

unlockPhysicalExtents

unmap

write

