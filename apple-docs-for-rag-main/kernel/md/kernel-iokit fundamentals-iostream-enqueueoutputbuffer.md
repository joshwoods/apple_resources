

- Kernel
- IOKit Fundamentals
- IOStream
-  enqueueOutputBuffer 

# enqueueOutputBuffer

A convenience method for enqueueing a buffer.

``` source
virtual IOReturn enqueueOutputBuffer(
 IOStreamBuffer *buffer, 
 IOByteCount dataOffset = 0, 
 IOByteCount dataLength = 0, 
 IOByteCount controlOffset = 0, 
 IOByteCount controlLength = 0); 
```

## Parameters 

`buffer`  

`dataOffset`  

`dataLength`  

`controlOffset`  

`controlLength`  

## See Also

### Queueing and dequeueing buffers

dequeueInputEntry

enqueueOutputEntry

