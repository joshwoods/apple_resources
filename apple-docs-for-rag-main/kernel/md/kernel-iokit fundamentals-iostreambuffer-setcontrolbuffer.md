

- Kernel
- IOKit Fundamentals
- IOStreamBuffer
-  setControlBuffer 

# setControlBuffer

Sets the control buffer for the IOStreamBuffer object.

``` source
virtual void setControlBuffer(
 IOMemoryDescriptor *controlBuffer); 
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

setDataBuffer

Sets the data buffer for the IOStreamBuffer object.

withMemoryDescriptors

