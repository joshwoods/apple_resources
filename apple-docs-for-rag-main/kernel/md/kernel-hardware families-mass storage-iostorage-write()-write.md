

- Kernel
- Hardware Families
- Mass Storage
- IOStorage
-  write() 

# write()

``` source
#ifdef __LP64__
 virtual void write(
 IOService *client, 
 UInt64 byteStart, 
 IOMemoryDescriptor *buffer, 
 IOStorageAttributes *attributes, 
 IOStorageCompletion *completion) = 0; 
#else /* !__LP64__ */
virtual void write(
 IOService *client, 
 UInt64 byteStart, 
 IOMemoryDescriptor *buffer, 
 IOStorageAttributes *attributes, 
 IOStorageCompletion *completion); 
#endif 
/* !__LP64__ */
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

## See Also

### Miscellaneous

complete

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

