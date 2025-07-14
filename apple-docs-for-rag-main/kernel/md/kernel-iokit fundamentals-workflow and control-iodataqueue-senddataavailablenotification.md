

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IODataQueue
-  sendDataAvailableNotification 

# sendDataAvailableNotification

Sends a dataAvailableNotification message to the specified mach port.

``` source
virtual void sendDataAvailableNotification(); 
```

## Overview

This method sends a message to the mach port passed to setNotificationPort(). It is used to indicate that data is available in the queue.

## See Also

### Miscellaneous

enqueue

Enqueues a new entry on the queue.

getMemoryDescriptor

Returns a memory descriptor covering the IODataQueueMemory region.

initWithCapacity

Initializes an IODataQueue instance with the capacity specified in the size parameter.

initWithEntries

Initializes an IODataQueue instance with the specified number of entries of the given size.

setNotificationPort

Creates a simple mach message targeting the mach port specified in port.

withCapacity

Static method that creates a new IODataQueue instance with the capacity specified in the size parameter.

withEntries

Static method that creates a new IODataQueue instance with the specified number of entries of the given size.

