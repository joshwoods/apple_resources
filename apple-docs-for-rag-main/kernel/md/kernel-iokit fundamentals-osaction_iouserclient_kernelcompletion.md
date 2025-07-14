

- Kernel
- IOKit Fundamentals
-  OSAction_IOUserClient_KernelCompletion 

Class

# OSAction_IOUserClient_KernelCompletion

macOS 11.0+

``` source
class OSAction_IOUserClient_KernelCompletion : OSAction, OSAction_IOUserClient_KernelCompletionInterface
```

## Topics

### Instance Methods

- Dispatch

- getMetaClass

## Relationships

### Inherits From

- OSAction
- OSAction_IOUserClient_KernelCompletionInterface

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

IOStreamBuffer

A class representing a data buffer that is part of an IOStream.

OSAction_IOUserClient_KernelCompletionInterface

