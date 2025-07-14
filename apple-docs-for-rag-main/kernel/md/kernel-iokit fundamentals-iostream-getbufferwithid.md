

- Kernel
- IOKit Fundamentals
- IOStream
-  getBufferWithID 

# getBufferWithID

``` source
virtual IOStreamBuffer *getBufferWithID(
 IOStreamBufferIDbufferID); 
```

## Parameters 

`bufferID`  

The ID of the buffer to get.

## Return Value

A pointer to an IOStreamBuffer object, or NULL if the buffer ID was invalid for this stream.

## See Also

### Managing buffers in an IOStream

addBuffer

Add a buffer to an IOStream.

addBuffers

getBufferCount

getBuffers

Get an array containing all the buffers in the stream.

removeAllBuffers()

removeAllBuffers()

removeBuffer(IOStreamBuffer *)

Removes a buffer from the stream. Buffers cannot be removed while the stream is open, as this will change the buffer IDs of existing buffers.

removeBuffer(IOStreamBufferID)

Removes a buffer from the stream. Buffers cannot be removed while the stream is open, as this will change the buffer IDs of existing buffers.

