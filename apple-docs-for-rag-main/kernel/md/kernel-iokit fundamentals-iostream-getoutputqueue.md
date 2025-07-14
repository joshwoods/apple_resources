

- Kernel
- IOKit Fundamentals
- IOStream
-  getOutputQueue 

# getOutputQueue

``` source
virtual IOStreamBufferQueue *getOutputQueue(
 void); 
```

## Return Value

A pointer to the output IOStreamBufferQueue structure for the stream, or NULL if the stream is not open and the queue has not been created yet.

## See Also

### Managing shared queues

createQueues

Creates the shared input and output queues, without regard to whether the stream is open or not. Normally this is called by handleOpen().

destroyQueues

Releases the shared input and output queues.

getInputQueue

getInputQueueMemoryDescriptor

getOutputQueueMemoryDescriptor

