

- Kernel
- IOKit Fundamentals
- IOStream
-  getBuffers 

# getBuffers

Get an array containing all the buffers in the stream.

``` source
virtual OSArray *getBuffers(
 void ); 
```

## Overview

Returns an OSArray containing all the buffers in the stream in order of their buffer ID.

## See Also

### Managing buffers in an IOStream

addBuffer

Add a buffer to an IOStream.

addBuffers

getBufferCount

getBufferWithID

removeAllBuffers()

removeAllBuffers()

removeBuffer(IOStreamBuffer *)

Removes a buffer from the stream. Buffers cannot be removed while the stream is open, as this will change the buffer IDs of existing buffers.

removeBuffer(IOStreamBufferID)

Removes a buffer from the stream. Buffers cannot be removed while the stream is open, as this will change the buffer IDs of existing buffers.

