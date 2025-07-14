

- Kernel
- Hardware Families
- Mass Storage
- IOPartitionScheme
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

handleClose

handleIsOpen

handleOpen

lockPhysicalExtents

read

synchronizeCache

unmap

write

