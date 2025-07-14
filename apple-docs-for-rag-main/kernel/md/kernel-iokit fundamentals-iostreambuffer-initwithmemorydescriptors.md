

- Kernel
- IOKit Fundamentals
- IOStreamBuffer
-  initWithMemoryDescriptors 

# initWithMemoryDescriptors

``` source
virtual bool initWithMemoryDescriptors(
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

receiveClientReference

sendClientReference

setBufferID

Sets the buffer identifier for the IOStreamBuffer object.

setControlBuffer

Sets the control buffer for the IOStreamBuffer object.

setDataBuffer

Sets the data buffer for the IOStreamBuffer object.

withMemoryDescriptors

