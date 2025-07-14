

- Kernel
- Hardware Families
- Mass Storage
- IOFilterScheme
-  read 

# read

``` source
virtual void read(
 IOService *client, 
 UInt64byteStart, 
 IOMemoryDescriptor *buffer, 
 IOStorageAttributes *attributes, 
 IOStorageCompletion *completion); 
```

## Parameters 

`client`  

Client requesting the read.

`byteStart`  

Starting byte offset for the data transfer.

`buffer`  

Buffer for the data transfer. The size of the buffer implies the size of the data transfer.

`attributes`  

Attributes of the data transfer. See IOStorageAttributes. It is the responsibility of the callee to maintain the information for the duration of the data transfer, as necessary.

`completion`  

Completion routine to call once the data transfer is complete. It is the responsibility of the callee to maintain the information for the duration of the data transfer, as necessary.

## Overview

Read data from the storage object at the specified byte offset into the specified buffer, asynchronously. When the read completes, the caller will be notified via the specified completion action.

The buffer will be retained for the duration of the read.

For simple filter schemes, the default behavior is to simply pass the read through to the provider media. More complex filter schemes such as RAID will need to do extra processing here.

## See Also

### Miscellaneous

copyPhysicalExtent

handleClose

handleIsOpen

handleOpen

lockPhysicalExtents

synchronizeCache

unlockPhysicalExtents

unmap

write

