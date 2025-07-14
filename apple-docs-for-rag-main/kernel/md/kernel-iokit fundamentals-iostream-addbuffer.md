

- Kernel
- IOKit Fundamentals
- IOStream
-  addBuffer 

# addBuffer

Add a buffer to an IOStream.

``` source
virtual IOReturn addBuffer(
 IOStreamBuffer *buffer); 
```

## Parameters 

`buffer`  

## Overview

Adds an IOStreamBuffer to an IOStream. It will be added to the end of the buffer array, so the buffer ID of existing buffers will not change.

## See Also

### Managing buffers in an IOStream

addBuffers

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

