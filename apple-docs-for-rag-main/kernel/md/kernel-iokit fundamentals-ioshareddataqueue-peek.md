

- Kernel
- IOKit Fundamentals
- IOSharedDataQueue
-  peek 

# peek

Used to peek at the next entry on the queue.

``` source
virtual IODataQueueEntry * peek(); 
```

## Return Value

Returns a pointer to the next IODataQueueEntry if one is available. 0 (NULL) is returned if the queue is empty.

## Overview

This function can be used to look at the next entry which allows the entry to be received without having to copy it with dequeue. In order to do this, call peek to get the entry. Then call dequeue with a NULL data pointer. That will cause the head to be moved to the next entry, but no memory to be copied.

## See Also

### Miscellaneous

dequeue

Dequeues the next available entry on the queue and copies it into the given data pointer.

getMemoryDescriptor

Returns a memory descriptor covering the IODataQueueMemory region.

initWithCapacity

Initializes an IOSharedDataQueue instance with the capacity specified in the size parameter.

withCapacity

Static method that creates a new IOSharedDataQueue instance with the capacity specified in the size parameter.

withEntries

Static method that creates a new IOSharedDataQueue instance with the specified number of entries of the given size.

