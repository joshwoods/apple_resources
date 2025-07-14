

- Kernel
- IOKit Fundamentals
- IOStreamBuffer
-  getControlBuffer 

# getControlBuffer

``` source
virtual IOMemoryDescriptor *getControlBuffer(
 void); 
```

## Return Value

A pointer to the IOMemoryDescriptor for the control buffer.

## See Also

### Miscellaneous

getBufferID

Gets the buffer identifier for the IOStreamBuffer object.

getClientReferenceCount

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

