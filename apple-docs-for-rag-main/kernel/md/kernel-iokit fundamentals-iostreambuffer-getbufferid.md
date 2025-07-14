

- Kernel
- IOKit Fundamentals
- IOStreamBuffer
-  getBufferID 

# getBufferID

Gets the buffer identifier for the IOStreamBuffer object.

``` source
virtual IOStreamBufferID getBufferID(
 void); 
```

## Overview

The buffer identifier is unique across all buffers in a stream.

## See Also

### Miscellaneous

getClientReferenceCount

getControlBuffer

getDataBuffer

initWithMemoryDescriptors

receiveClientReference

sendClientReference

setBufferID

Sets the buffer identifier for the IOStreamBuffer object.

setControlBuffer

Sets the control buffer for the IOStreamBuffer object.

setDataBuffer

Sets the data buffer for the IOStreamBuffer object.

withMemoryDescriptors

