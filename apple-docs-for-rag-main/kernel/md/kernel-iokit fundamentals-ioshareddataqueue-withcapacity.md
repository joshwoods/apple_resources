

- Kernel
- IOKit Fundamentals
- IOSharedDataQueue
-  withCapacity 

# withCapacity

Static method that creates a new IOSharedDataQueue instance with the capacity specified in the size parameter.

``` source
static IOSharedDataQueue *withCapacity(
 UInt32size); 
```

## Parameters 

`size`  

The size of the data queue memory region.

## Return Value

Returns the newly allocated IOSharedDataQueue instance. Zero is returned on failure.

## Overview

The actual size of the entire data queue memory region (to be shared into a user process) is equal to the capacity plus the IODataQueueMemory overhead. This overhead value can be determined from the DATA_QUEUE_MEMORY_HEADER_SIZE macro in \. The size of the data queue memory region must include space for the overhead of each IODataQueueEntry. This entry overhead can be determined from the DATA_QUEUE_ENTRY_HEADER_SIZE macro in \.

This method allocates a new IODataQueue instance and then calls initWithCapacity() with the given size parameter. If the initWithCapacity() fails, the new instance is released and zero is returned.

## See Also

### Miscellaneous

dequeue

Dequeues the next available entry on the queue and copies it into the given data pointer.

getMemoryDescriptor

Returns a memory descriptor covering the IODataQueueMemory region.

initWithCapacity

Initializes an IOSharedDataQueue instance with the capacity specified in the size parameter.

peek

Used to peek at the next entry on the queue.

withEntries

Static method that creates a new IOSharedDataQueue instance with the specified number of entries of the given size.

