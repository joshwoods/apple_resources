

- Kernel
- IOKit Fundamentals
- IOStream
-  getOutputQueueMemoryDescriptor 

# getOutputQueueMemoryDescriptor

``` source
virtual IOMemoryDescriptor *getOutputQueueMemoryDescriptor(
 void); 
```

## Return Value

An IOMemoryDescriptor object repesenting the shared memory output queue buffer.

## See Also

### Managing shared queues

createQueues

Creates the shared input and output queues, without regard to whether the stream is open or not. Normally this is called by handleOpen().

destroyQueues

Releases the shared input and output queues.

getInputQueue

getInputQueueMemoryDescriptor

getOutputQueue

