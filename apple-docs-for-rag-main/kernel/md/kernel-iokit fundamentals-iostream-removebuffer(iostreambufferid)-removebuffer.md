

- Kernel
- IOKit Fundamentals
- IOStream
-  removeBuffer(IOStreamBufferID) 

# removeBuffer(IOStreamBufferID)

Removes a buffer from the stream. Buffers cannot be removed while the stream is open, as this will change the buffer IDs of existing buffers.

``` source
virtual IOReturn removeBuffer(
 IOStreamBufferIDbufferID); 
```

## Parameters 

`bufferID`  

The ID of the buffer to remove.

## Return Value

Returns kIOReturnSuccess if the buffer was removed.

## See Also

### Managing buffers in an IOStream

addBuffer

Add a buffer to an IOStream.

addBuffers

getBufferCount

getBuffers

Get an array containing all the buffers in the stream.

getBufferWithID

removeAllBuffers()

removeAllBuffers()

removeBuffer(IOStreamBuffer *)

Removes a buffer from the stream. Buffers cannot be removed while the stream is open, as this will change the buffer IDs of existing buffers.

