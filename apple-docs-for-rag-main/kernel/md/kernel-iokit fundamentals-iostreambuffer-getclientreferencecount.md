

- Kernel
- IOKit Fundamentals
- IOStreamBuffer
-  getClientReferenceCount 

# getClientReferenceCount

``` source
virtual SInt32 getClientReferenceCount(
 void ); 
```

## Return Value

The count of client references to this buffer. It may be positive or negative, depending on whether the client is sending data into the kernel, or the kernel is sending data out to the client.

## See Also

### Miscellaneous

getBufferID

Gets the buffer identifier for the IOStreamBuffer object.

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

