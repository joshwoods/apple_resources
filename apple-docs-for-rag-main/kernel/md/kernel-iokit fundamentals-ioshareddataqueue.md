

- Kernel
- IOKit Fundamentals
-  IOSharedDataQueue 

Class

# IOSharedDataQueue

A generic queue designed to pass data both from the kernel to a user process and from a user process to the kernel.

macOS 10.5+

``` source
class IOSharedDataQueue : IODataQueue
```

## Overview

The IOSharedDataQueue class is designed to also allow a user process to queue data to kernel code. IOSharedDataQueue objects are designed to be used in a single producer / single consumer situation. As such, there are no locks on the data itself. Because the kernel enqueue and user-space dequeue methods follow a strict set of guidelines, no locks are necessary to maintain the integrity of the data struct.

Each data entry can be variable sized, but the entire size of the queue data region (including overhead for each entry) must be specified up front.

In order for the IODataQueue instance to notify the user process that data is available, a notification mach port must be set. When the queue is empty and a new entry is added, a message is sent to the specified port.

In order to make the data queue memory available to a user process, the method getMemoryDescriptor() must be used to get an IOMemoryDescriptor instance that can be mapped into a user process. Typically, the clientMemoryForType() method on an IOUserClient instance will be used to request the IOMemoryDescriptor and then return it to be mapped into the user process.

## Topics

### Miscellaneous

dequeue

Dequeues the next available entry on the queue and copies it into the given data pointer.

getMemoryDescriptor

Returns a memory descriptor covering the IODataQueueMemory region.

initWithCapacity

Initializes an IOSharedDataQueue instance with the capacity specified in the size parameter.

peek

Used to peek at the next entry on the queue.

withCapacity

Static method that creates a new IOSharedDataQueue instance with the capacity specified in the size parameter.

withEntries

Static method that creates a new IOSharedDataQueue instance with the specified number of entries of the given size.

### Instance Variables

_reserved

### Instance Methods

- dequeue

- enqueue

- free

- getMemoryDescriptor

- getMetaClass

- getQueueSize

- initWithCapacity

- peek

- setQueueSize

### Type Methods

+ withCapacity

+ withEntries

## Relationships

### Inherits From

- IODataQueue

## See Also

### User-Space Interactions

IOSharedInterruptController

IOUserClient

Provides a basis for communication between client applications and I/O Kit objects.

IOStreamUserClient

IOStream

A class representing a stream of data buffers passed from kernel to user space and back again.

IOStreamBuffer

A class representing a data buffer that is part of an IOStream.

OSAction_IOUserClient_KernelCompletion

OSAction_IOUserClient_KernelCompletionInterface

