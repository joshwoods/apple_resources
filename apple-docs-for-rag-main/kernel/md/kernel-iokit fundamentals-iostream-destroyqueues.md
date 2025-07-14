

- Kernel
- IOKit Fundamentals
- IOStream
-  destroyQueues 

# destroyQueues

Releases the shared input and output queues.

``` source
virtual IOReturn destroyQueues(
 void ); 
```

## Return Value

Returns kIOReturnSuccess if the queues were successfully destroyed. The queues cannot be destroyed while the stream is open by a client.

## See Also

### Managing shared queues

createQueues

Creates the shared input and output queues, without regard to whether the stream is open or not. Normally this is called by handleOpen().

getInputQueue

getInputQueueMemoryDescriptor

getOutputQueue

getOutputQueueMemoryDescriptor

