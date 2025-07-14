

- Kernel
- IOKit Fundamentals
- IOStream
-  addBuffers 

# addBuffers

``` source
virtual IOReturn addBuffers(
 OSArray *buffers); 
```

## Parameters 

`buffers`  

## See Also

### Managing buffers in an IOStream

addBuffer

Add a buffer to an IOStream.

getBufferCount

getBuffers

Get an array containing all the buffers in the stream.

getBufferWithID

removeAllBuffers()

removeAllBuffers()

removeBuffer(IOStreamBuffer *)

Removes a buffer from the stream. Buffers cannot be removed while the stream is open, as this will change the buffer IDs of existing buffers.

removeBuffer(IOStreamBufferID)

Removes a buffer from the stream. Buffers cannot be removed while the stream is open, as this will change the buffer IDs of existing buffers.

