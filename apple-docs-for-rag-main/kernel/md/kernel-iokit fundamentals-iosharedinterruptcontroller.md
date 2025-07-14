

- Kernel
- IOKit Fundamentals
-  IOSharedInterruptController 

Class

# IOSharedInterruptController

macOS 10.0+

``` source
class IOSharedInterruptController : IOInterruptController
```

## Topics

### Instance Methods

- disableInterrupt

- enableInterrupt

- getInterruptHandlerAddress

- getInterruptType

- getMetaClass

- handleInterrupt

- initInterruptController

- registerInterrupt

- unregisterInterrupt

## Relationships

### Inherits From

- IOInterruptController

## See Also

### User-Space Interactions

IOSharedDataQueue

A generic queue designed to pass data both from the kernel to a user process and from a user process to the kernel.

IOUserClient

Provides a basis for communication between client applications and I/O Kit objects.

IOStreamUserClient

IOStream

A class representing a stream of data buffers passed from kernel to user space and back again.

IOStreamBuffer

A class representing a data buffer that is part of an IOStream.

OSAction_IOUserClient_KernelCompletion

OSAction_IOUserClient_KernelCompletionInterface

