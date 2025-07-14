

- Kernel
- IOKit Fundamentals
- IOSharedDataQueue
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

dequeue

Dequeues the next available entry on the queue and copies it into the given data pointer.

initWithCapacity

Initializes an IOSharedDataQueue instance with the capacity specified in the size parameter.

peek

Used to peek at the next entry on the queue.

withCapacity

Static method that creates a new IOSharedDataQueue instance with the capacity specified in the size parameter.

withEntries

Static method that creates a new IOSharedDataQueue instance with the specified number of entries of the given size.

