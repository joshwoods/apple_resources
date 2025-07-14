

- Kernel
- IOKit Fundamentals
- IOStreamBuffer
-  withMemoryDescriptors 

# withMemoryDescriptors

``` source
static IOStreamBuffer *withMemoryDescriptors(
 IOMemoryDescriptor *dataBuffer, 
 IOMemoryDescriptor *controlBuffer, 
 IOStreamBufferID bufferID = 0); 
```

## See Also

### Miscellaneous

getBufferID

Gets the buffer identifier for the IOStreamBuffer object.

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

