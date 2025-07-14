

- Kernel
- Hardware Families
- Mass Storage
- IOStorage
-  open 

# open

``` source
virtual bool open(
 IOService *client, 
 IOOptionBitsoptions, 
 IOStorageAccessaccess); 
```

## Parameters 

`client`  

Client requesting the open.

`options`  

Options for the open. Set to zero.

`access`  

Access level for the open. Set to kIOStorageAccessReader or kIOStorageAccessReaderWriter.

## Return Value

Returns true if the open was successful, false otherwise.

## Overview

Ask the storage object for permission to access its contents; the method is equivalent to IOService::open(), but with the correct parameter types.

This method may also be invoked to upgrade or downgrade the access of an existing open (if it fails, the existing open prevails).

## See Also

### Miscellaneous

complete

copyPhysicalExtent

handleClose

handleIsOpen

handleOpen

lockPhysicalExtents

read()

read()

synchronizeCache

unlockPhysicalExtents

unmap

write()

write()

