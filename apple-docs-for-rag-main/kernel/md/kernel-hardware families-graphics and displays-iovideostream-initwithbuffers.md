

- Kernel
- Hardware Families
- Graphics and Displays
- IOVideoStream
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

`buffers`  

An array of IOStreamBuffer objects which will be the buffers for this stream.

`mode`  

The initial mode of the video stream, either output, input, or input/output.

`queueLength`  

The nuber of queue entries to reserve in the input and output queue. Zero means to make the queues big enough to accommodate all the buffers at once.

`properties`  

A dictionary of properties which will be set on the video stream.

## See Also

### Miscellaneous

getStreamMode

Returns the mode of the stream, either input or output.

setStreamMode

Sets the mode of the stream, either input or output.

startStream

Start sending data on a stream.

stopStream

Stop sending data on a stream.

suspendStream

Temporarily suspend data flow on the stream.

withBuffers

