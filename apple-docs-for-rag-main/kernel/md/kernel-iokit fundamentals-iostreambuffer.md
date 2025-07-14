

- Kernel
- IOKit Fundamentals
-  IOStreamBuffer 

Class

# IOStreamBuffer

A class representing a data buffer that is part of an IOStream.

macOS 10.5+

``` source
class IOStreamBuffer : OSObject
```

## Topics

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

withMemoryDescriptors

### Instance Methods

- free

- getBufferID

- getClientReferenceCount

- getControlBuffer

- getDataBuffer

- getMetaClass

- initWithMemoryDescriptors

- receiveClientReference

- sendClientReference

- setBufferID

- setControlBuffer

- setDataBuffer

### Type Methods

+ withMemoryDescriptors

## Relationships

### Inherits From

- OSObject

## See Also

### User-Space Interactions

IOSharedDataQueue

A generic queue designed to pass data both from the kernel to a user process and from a user process to the kernel.

IOSharedInterruptController

IOUserClient

Provides a basis for communication between client applications and I/O Kit objects.

IOStreamUserClient

IOStream

A class representing a stream of data buffers passed from kernel to user space and back again.

OSAction_IOUserClient_KernelCompletion

OSAction_IOUserClient_KernelCompletionInterface

