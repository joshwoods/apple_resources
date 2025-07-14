

- Kernel
- IOKit Fundamentals
- IOStreamBuffer
-  getDataBuffer 

# getDataBuffer

``` source
virtual IOMemoryDescriptor *getDataBuffer(
 void); 
```

## Return Value

A pointer to the IOMemoryDescriptor for the data buffer.

## See Also

### Miscellaneous

getBufferID

Gets the buffer identifier for the IOStreamBuffer object.

getClientReferenceCount

getControlBuffer

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

