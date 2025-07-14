

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IODataQueue
-  setNotificationPort 

# setNotificationPort

Creates a simple mach message targeting the mach port specified in port.

``` source
virtual void setNotificationPort(
 mach_port_tport); 
```

## Parameters 

`port`  

The mach port to target with the notification message.

## Overview

This message is sent when data is added to an empty queue. It is to notify a user process that new data has become available.

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

sendDataAvailableNotification

Sends a dataAvailableNotification message to the specified mach port.

withCapacity

Static method that creates a new IODataQueue instance with the capacity specified in the size parameter.

withEntries

Static method that creates a new IODataQueue instance with the specified number of entries of the given size.

