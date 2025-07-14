

- Kernel
- Hardware Families
- Mass Storage
- IOFilterScheme
-  handleOpen 

# handleOpen

``` source
virtual bool handleOpen(
 IOService *client, 
 IOOptionBitsoptions, 
 void *access); 
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

The handleOpen method grants or denies permission to access this object to an interested client. The argument is an IOStorageAccess value that specifies the level of access desired -- reader or reader-writer.

This method can be invoked to upgrade or downgrade the access level for an existing client as well. The previous access level will prevail for upgrades that fail, of course. A downgrade should never fail. If the new access level should be the same as the old for a given client, this method will do nothing and return success. In all cases, one, singular close-per-client is expected for all opens-per-client received.

This implementation replaces the IOService definition of handleOpen().

## See Also

### Miscellaneous

copyPhysicalExtent

handleClose

handleIsOpen

lockPhysicalExtents

read

synchronizeCache

unlockPhysicalExtents

unmap

write

