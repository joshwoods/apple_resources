

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IODataQueue
-  initWithCapacity 

# initWithCapacity

Initializes an IODataQueue instance with the capacity specified in the size parameter.

``` source
virtual Boolean initWithCapacity(
 UInt32size); 
```

## Parameters 

`size`  

The size of the data queue memory region.

## Return Value

Returns true on success and false on failure.

## Overview

The actual size of the entire data queue memory region (to be shared into a user process) is equal to the capacity plus the IODataQueueMemory overhead. This overhead value can be determined from the DATA_QUEUE_MEMORY_HEADER_SIZE macro in \. The size of the data queue memory region must include space for the overhead of each IODataQueueEntry. This entry overhead can be determined from the DATA_QUEUE_ENTRY_HEADER_SIZE macro in \.

## See Also

### Miscellaneous

enqueue

Enqueues a new entry on the queue.

getMemoryDescriptor

Returns a memory descriptor covering the IODataQueueMemory region.

initWithEntries

Initializes an IODataQueue instance with the specified number of entries of the given size.

sendDataAvailableNotification

Sends a dataAvailableNotification message to the specified mach port.

setNotificationPort

Creates a simple mach message targeting the mach port specified in port.

withCapacity

Static method that creates a new IODataQueue instance with the capacity specified in the size parameter.

withEntries

Static method that creates a new IODataQueue instance with the specified number of entries of the given size.

