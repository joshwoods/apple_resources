

- Kernel
- IOKit Fundamentals
- IOStream
-  initWithBuffers 

# initWithBuffers

``` source
virtual bool initWithBuffers(
 OSArray *buffers,
 IOStreamMode mode = kIOStreamModeOutput,
 IOItemCount queueLength = 0,
 OSDictionary *properties = 0); 
```

## Parameters 

`mode`  

The initial mode of the stream, either output, input, or input/output.

`queueLength`  

The nuber of queue entries to reserve in the input and output queue. Zero means to make the queues big enough to accommodate all the buffers at once.

`properties`  

A dictionary of properties which will be set on the stream.

`buffers`  

An array of IOStreamBuffer objects which will be the buffers for this stream.

## See Also

### Creating IOStream objects

free

withBuffers

