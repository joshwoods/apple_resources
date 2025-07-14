

- Kernel
- Hardware Families
- Mass Storage
- IOFilterScheme
-  handleIsOpen 

# handleIsOpen

``` source
virtual bool handleIsOpen(
 const IOService *client) const; 
```

## Parameters 

`client`  

Client to check the open state of. Set to zero to check the open state of all clients.

## Return Value

Returns true if the client was (or clients were) open, false otherwise.

## Overview

The handleIsOpen method determines whether the specified client, or any client if none is specified, presently has an open on this object.

This implementation replaces the IOService definition of handleIsOpen().

## See Also

### Miscellaneous

copyPhysicalExtent

handleClose

handleOpen

lockPhysicalExtents

read

synchronizeCache

unlockPhysicalExtents

unmap

write

