

- Kernel
- Hardware Families
- Mass Storage
- IOStorage
-  handleClose 

# handleClose

``` source
virtual void handleClose(
 IOService *client,
 IOOptionBitsoptions) = 0; 
```

## Parameters 

`client`  

Client requesting the close.

`options`  

Options for the close. Set to zero.

## Overview

The handleClose method closes the client's access to this object.

## See Also

### Miscellaneous

complete

copyPhysicalExtent

handleIsOpen

handleOpen

lockPhysicalExtents

open

read()

read()

synchronizeCache

unlockPhysicalExtents

unmap

write()

write()

