

- Kernel
- Hardware Families
- Mass Storage
- IOPartitionScheme
-  write 

# write

``` source
virtual void write(
 IOService *client, 
 UInt64byteStart, 
 IOMemoryDescriptor *buffer, 
 IOStorageAttributes *attributes, 
 IOStorageCompletion *completion); 
```

## Parameters 

`client`  

Client requesting the write.

`byteStart`  

Starting byte offset for the data transfer.

`buffer`  

Buffer for the data transfer. The size of the buffer implies the size of the data transfer.

`attributes`  

Attributes of the data transfer. See IOStorageAttributes. It is the responsibility of the callee to maintain the information for the duration of the data transfer, as necessary.

`completion`  

Completion routine to call once the data transfer is complete. It is the responsibility of the callee to maintain the information for the duration of the data transfer, as necessary.

## Overview

Write data into the storage object at the specified byte offset from the specified buffer, asynchronously. When the write completes, the caller will be notified via the specified completion action.

The buffer will be retained for the duration of the write.

For simple partition schemes, the default behavior is to simply pass the write through to the provider media. More complex partition schemes such as RAID will need to do extra processing here.

## See Also

### Miscellaneous

copyPhysicalExtent

handleClose

handleIsOpen

handleOpen

lockPhysicalExtents

read

synchronizeCache

unlockPhysicalExtents

unmap

