

- Kernel
- IOKit Fundamentals
-  IOStreamUserClient 

Class

# IOStreamUserClient

macOS 10.5+

``` source
class IOStreamUserClient : IOUserClient
```

## Topics

### Instance Methods

- clientClose

- clientDied

- clientMemoryForType

- clientMemoryForTypeGated

- closeMethod

- connectClient

- free

- getBufferCountMethod

- getMetaClass

- getModeMethod

- getService

- getTargetAndMethodForIndex

- getTargetAndMethodForIndexGated

- getTargetAndTrapForIndex

- initWithTask

- initWithTask

- inputSyncTrap

- inputTrap

- openMethod

- registerNotificationPort

- setModeMethod

- start

- startMethod

- stop

- stopMethod

- suspendMethod

## Relationships

### Inherits From

- IOUserClient

## See Also

### User-Space Interactions

IOSharedDataQueue

A generic queue designed to pass data both from the kernel to a user process and from a user process to the kernel.

IOSharedInterruptController

IOUserClient

Provides a basis for communication between client applications and I/O Kit objects.

IOStream

A class representing a stream of data buffers passed from kernel to user space and back again.

IOStreamBuffer

A class representing a data buffer that is part of an IOStream.

OSAction_IOUserClient_KernelCompletion

OSAction_IOUserClient_KernelCompletionInterface

