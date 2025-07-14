

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IODataQueue
-  withEntries 

# withEntries

Static method that creates a new IODataQueue instance with the specified number of entries of the given size.

``` source
static IODataQueue *withEntries(
 UInt32numEntries,
 UInt32entrySize); 
```

## Parameters 

`numEntries`  

Number of entries to allocate space for.

`entrySize`  

Size of each entry.

## Return Value

Reeturns the newly allocated IODataQueue instance. Zero is returned on failure.

## Overview

This method will create a new IODataQueue instance with enough capacity for numEntries of entrySize. It does account for the IODataQueueEntry overhead for each entry. Note that the numEntries and entrySize are simply used to determine the data region size. They do not actually restrict the size of number of entries that can be added to the queue.

This method allocates a new IODataQueue instance and then calls initWithEntries() with the given numEntries and entrySize parameters. If the initWithEntries() fails, the new instance is released and zero is returned.

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

setNotificationPort

Creates a simple mach message targeting the mach port specified in port.

withCapacity

Static method that creates a new IODataQueue instance with the capacity specified in the size parameter.

