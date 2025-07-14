

- Kernel
- Hardware Families
- Mass Storage
- IOStorage
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

unmap

write()

write()

