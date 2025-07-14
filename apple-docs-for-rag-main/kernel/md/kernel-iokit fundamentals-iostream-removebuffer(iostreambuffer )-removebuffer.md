

- Kernel
- IOKit Fundamentals
- IOStream
-  removeBuffer(IOStreamBuffer \*) 

# removeBuffer(IOStreamBuffer \*)

Removes a buffer from the stream. Buffers cannot be removed while the stream is open, as this will change the buffer IDs of existing buffers.

``` source
virtual IOReturn removeBuffer(
 IOStreamBuffer *buffer); 
```

## Parameters 

`buffer`  

A pointer to an IOStreamBuffer object in the stream.

## Return Value

Returns kIOReturnSuccess if the buffer was removed, or kIOReturnNotFound if the buffer was not in this stream.

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

removeBuffer(IOStreamBufferID)

Removes a buffer from the stream. Buffers cannot be removed while the stream is open, as this will change the buffer IDs of existing buffers.

