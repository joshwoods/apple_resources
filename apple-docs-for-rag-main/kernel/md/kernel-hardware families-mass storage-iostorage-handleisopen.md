

- Kernel
- Hardware Families
- Mass Storage
- IOStorage
-  handleIsOpen 

# handleIsOpen

``` source
virtual bool handleIsOpen(
 const IOService *client) const = 0; 
```

## Parameters 

`client`  

Client to check the open state of. Set to zero to check the open state of all clients.

## Return Value

Returns true if the client was (or clients were) open, false otherwise.

## Overview

The handleIsOpen method determines whether the specified client, or any client if none is specified, presently has an open on this object.

## See Also

### Miscellaneous

complete

copyPhysicalExtent

handleClose

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

