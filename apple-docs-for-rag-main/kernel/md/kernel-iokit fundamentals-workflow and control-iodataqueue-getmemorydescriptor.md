

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IODataQueue
-  getMemoryDescriptor 

# getMemoryDescriptor

Returns a memory descriptor covering the IODataQueueMemory region.

``` source
virtual IOMemoryDescriptor *getMemoryDescriptor(); 
```

## Return Value

Returns a newly allocated IOMemoryDescriptor for the IODataQueueMemory region. Returns zero on failure.

## Overview

The IOMemoryDescriptor instance returned by this method is intended to be mapped into a user process. This is the memory region that the IODataQueueClient code operates on.

## See Also

### Miscellaneous

enqueue

Enqueues a new entry on the queue.

initWithCapacity

Initializes an IODataQueue instance with the capacity specified in the size parameter.

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

