

- Kernel
- Hardware Families
- Mass Storage
- IOStorage
-  copyPhysicalExtent 

# copyPhysicalExtent

``` source
virtual IOStorage * copyPhysicalExtent(
 IOService *client, 
 UInt64 *byteStart, 
 UInt64 *byteCount); 
```

## Parameters 

`client`  

Client requesting the operation.

`byteStart`  

Starting byte offset for the operation. Returns a physical byte offset, relative to the physical storage object, on success.

`byteCount`  

Size of the operation. Returns the actual number of bytes which can be transferred, relative to the physical storage object, on success.

## Return Value

A reference to the physical storage object, which should be released by the caller, or a null on error.

## Overview

Convert the specified byte offset into a physical byte offset, relative to a physical storage object. This call should only be made within the context of lockPhysicalExtents().

## See Also

### Miscellaneous

complete

handleClose

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

