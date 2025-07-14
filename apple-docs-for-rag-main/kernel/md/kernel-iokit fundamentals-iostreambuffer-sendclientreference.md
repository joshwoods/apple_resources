

- Kernel
- IOKit Fundamentals
- IOStreamBuffer
-  sendClientReference 

# sendClientReference

``` source
virtual SInt32 sendClientReference(
 IOByteCount offset = 0,
 IOByteCount length = 0 ); 
```

## Parameters 

`offset`  

The offset in the buffer of the data sent to the client.

`length`  

The length of the data sent to the client.

## Return Value

The new client reference count.

## See Also

### Miscellaneous

getBufferID

Gets the buffer identifier for the IOStreamBuffer object.

getClientReferenceCount

getControlBuffer

getDataBuffer

initWithMemoryDescriptors

receiveClientReference

setBufferID

Sets the buffer identifier for the IOStreamBuffer object.

setControlBuffer

Sets the control buffer for the IOStreamBuffer object.

setDataBuffer

Sets the data buffer for the IOStreamBuffer object.

withMemoryDescriptors

