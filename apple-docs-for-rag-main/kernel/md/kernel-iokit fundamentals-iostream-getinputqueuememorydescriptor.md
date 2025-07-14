

- Kernel
- IOKit Fundamentals
- IOStream
-  getInputQueueMemoryDescriptor 

# getInputQueueMemoryDescriptor

``` source
virtual IOMemoryDescriptor *getInputQueueMemoryDescriptor(
 void); 
```

## Return Value

An IOMemoryDescriptor object repesenting the shared memory input queue buffer.

## See Also

### Managing shared queues

createQueues

Creates the shared input and output queues, without regard to whether the stream is open or not. Normally this is called by handleOpen().

destroyQueues

Releases the shared input and output queues.

getInputQueue

getOutputQueue

getOutputQueueMemoryDescriptor

