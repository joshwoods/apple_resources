

- Kernel
- Hardware Families
- Mass Storage
- IOStorage
-  complete 

# complete

``` source
static void complete(
 IOStorageCompletion *completion, 
 IOReturn status, 
 UInt64 actualByteCount = 0); 
```

## Parameters 

`completion`  

Completion information for the data transfer.

`status`  

Status of the data transfer.

`actualByteCount`  

Actual number of bytes transferred in the data transfer.

## Overview

Invokes the specified completion action of the read/write request. If the completion action is unspecified, no action is taken. This method serves simply as a convenience to storage subclass developers.

## See Also

### Miscellaneous

copyPhysicalExtent

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

