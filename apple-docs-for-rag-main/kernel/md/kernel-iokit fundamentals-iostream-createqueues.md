

- Kernel
- IOKit Fundamentals
- IOStream
-  createQueues 

# createQueues

Creates the shared input and output queues, without regard to whether the stream is open or not. Normally this is called by handleOpen().

``` source
virtual IOReturn createQueues(
 IOItemCount queueLength = 0,
 IOOptionBits options = 0 ); 
```

## Parameters 

`queueLength`  

`options`  

## Return Value

Returns kIOReturnSuccess if the queues were successfully created.

## See Also

### Managing shared queues

destroyQueues

Releases the shared input and output queues.

getInputQueue

getInputQueueMemoryDescriptor

getOutputQueue

getOutputQueueMemoryDescriptor

