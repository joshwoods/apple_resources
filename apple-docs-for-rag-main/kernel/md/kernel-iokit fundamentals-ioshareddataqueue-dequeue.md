

- Kernel
- IOKit Fundamentals
- IOSharedDataQueue
-  dequeue 

# dequeue

Dequeues the next available entry on the queue and copies it into the given data pointer.

``` source
virtual Boolean dequeue(
 void *data,
 UInt32 *dataSize); 
```

## Parameters 

`data`  

A pointer to the data memory region in which to copy the next entry data on the queue. If this parameter is 0 (NULL), it will simply move to the next entry.

`dataSize`  

A pointer to the size of the data parameter. On return, this contains the size of the actual entry data - even if the original size was not large enough.

## Return Value

Returns true on success and false on failure. Typically failure means that the queue is empty.

## Overview

This function will dequeue the next available entry on the queue. If a data pointer is provided, it will copy the data into the memory region if there is enough space available as specified in the dataSize parameter. If no data pointer is provided, it will simply move the head value past the current entry.

## See Also

### Miscellaneous

getMemoryDescriptor

Returns a memory descriptor covering the IODataQueueMemory region.

initWithCapacity

Initializes an IOSharedDataQueue instance with the capacity specified in the size parameter.

peek

Used to peek at the next entry on the queue.

withCapacity

Static method that creates a new IOSharedDataQueue instance with the capacity specified in the size parameter.

withEntries

Static method that creates a new IOSharedDataQueue instance with the specified number of entries of the given size.

