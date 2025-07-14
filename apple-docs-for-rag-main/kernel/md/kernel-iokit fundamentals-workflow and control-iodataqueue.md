

- Kernel
- IOKit Fundamentals
- Workflow and Control
-  IODataQueue 

Class

# IODataQueue

A generic queue designed to pass data from the kernel to a user process.

macOS 10.0+

``` source
class IODataQueue : OSObject
```

## Overview

The IODataQueue class is designed to allow kernel code to queue data to a user process. IODataQueue objects are designed to be used in a single producer / single consumer situation. As such, there are no locks on the data itself. Because the kernel enqueue and user-space dequeue methods follow a strict set of guidelines, no locks are necessary to maintain the integrity of the data struct.

Each data entry can be variable sized, but the entire size of the queue data region (including overhead for each entry) must be specified up front.

In order for the IODataQueue instance to notify the user process that data is available, a notification mach port must be set. When the queue is empty and a new entry is added, a message is sent to the specified port.

User client code exists in the IOKit framework that facilitates the creation of the receive notification port as well as the listen process for new data available notifications.

In order to make the data queue memory available to a user process, the method getMemoryDescriptor() must be used to get an IOMemoryDescriptor instance that can be mapped into a user process. Typically, the clientMemoryForType() method on an IOUserClient instance will be used to request the IOMemoryDescriptor and then return it to be mapped into the user process.

## Topics

### Miscellaneous

enqueue

Enqueues a new entry on the queue.

getMemoryDescriptor

Returns a memory descriptor covering the IODataQueueMemory region.

initWithCapacity

Initializes an IODataQueue instance with the capacity specified in the size parameter.

initWithEntries

Initializes an IODataQueue instance with the specified number of entries of the given size.

sendDataAvailableNotification

Sends a dataAvailableNotification message to the specified mach port.

setNotificationPort

Creates a simple mach message targeting the mach port specified in port.

withCapacity

Static method that creates a new IODataQueue instance with the capacity specified in the size parameter.

withEntries

Static method that creates a new IODataQueue instance with the specified number of entries of the given size.

### Instance Methods

- enqueue

- free

- getMemoryDescriptor

- getMetaClass

- initWithCapacity

- initWithEntries

- sendDataAvailableNotification

- setNotificationPort

### Type Methods

+ withCapacity

+ withEntries

## Relationships

### Inherits From

- OSObject

## See Also

### Data Queues

IODataQueueDispatchSource

IODataQueueDispatchSourceInterface

