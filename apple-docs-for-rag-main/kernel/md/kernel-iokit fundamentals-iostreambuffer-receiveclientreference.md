

- Kernel
- IOKit Fundamentals
- IOStreamBuffer
-  receiveClientReference 

# receiveClientReference

``` source
virtual SInt32 receiveClientReference(
 IOByteCount offset = 0,
 IOByteCount length = 0 ); 
```

## Parameters 

`offset`  

The offset in the buffer of the data from the client.

`length`  

The length of the data from the client.

## See Also

### Miscellaneous

getBufferID

Gets the buffer identifier for the IOStreamBuffer object.

getClientReferenceCount

getControlBuffer

getDataBuffer

initWithMemoryDescriptors

sendClientReference

setBufferID

Sets the buffer identifier for the IOStreamBuffer object.

setControlBuffer

Sets the control buffer for the IOStreamBuffer object.

setDataBuffer

Sets the data buffer for the IOStreamBuffer object.

withMemoryDescriptors

