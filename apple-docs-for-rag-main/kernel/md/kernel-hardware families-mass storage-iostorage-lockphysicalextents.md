

- Kernel
- Hardware Families
- Mass Storage
- IOStorage
-  lockPhysicalExtents 

# lockPhysicalExtents

``` source
virtual bool lockPhysicalExtents(
 IOService *client); 
```

## Parameters 

`client`  

Client requesting the operation.

## Return Value

Returns true if the lock was successful, false otherwise.

## Overview

Lock the contents of the storage object against relocation temporarily, for the purpose of getting physical extents.

## See Also

### Miscellaneous

complete

copyPhysicalExtent

handleClose

handleIsOpen

handleOpen

open

read()

read()

synchronizeCache

unlockPhysicalExtents

unmap

write()

write()

