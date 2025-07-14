

- Kernel
- IOKit Fundamentals
- IOSharedDataQueue
-  initWithCapacity 

# initWithCapacity

Initializes an IOSharedDataQueue instance with the capacity specified in the size parameter.

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

The actual size of the entire data queue memory region (to be shared into a user process) is equal to the capacity plus the IODataQueueMemory overhead. This overhead value can be determined from the DATA_QUEUE_MEMORY_HEADER_SIZE and DATA_QUEUE_MEMORY_APPENDIX_SIZE macro in \. The size of the data queue memory region must include space for the overhead of each IODataQueueEntry. This entry overhead can be determined from the DATA_QUEUE_ENTRY_HEADER_SIZE macro in \.

## See Also

### Miscellaneous

dequeue

Dequeues the next available entry on the queue and copies it into the given data pointer.

getMemoryDescriptor

Returns a memory descriptor covering the IODataQueueMemory region.

peek

Used to peek at the next entry on the queue.

withCapacity

Static method that creates a new IOSharedDataQueue instance with the capacity specified in the size parameter.

withEntries

Static method that creates a new IOSharedDataQueue instance with the specified number of entries of the given size.

