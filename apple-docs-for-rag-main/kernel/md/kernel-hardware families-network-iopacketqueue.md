

- Kernel
- Hardware Families
- Network
-  IOPacketQueue 

Class

# IOPacketQueue

Implements a bounded FIFO queue of mbuf packets.

macOS 10.0+

``` source
class IOPacketQueue : OSObject
```

## Overview

Packets are removed from the head of the queue (dequeue), and new packets are added to the tail of the queue (enqueue). A spinlock is used to synchronize access to the queue between methods that have a "lock" prefix.

## Topics

### Miscellaneous

dequeue

Removes a single packet from the head of the queue.

dequeueAll

Removes all packets from the queue and returns the head of the packet chain.

enqueue(IOPacketQueue *)

Removes all packets from the specified queue, and adds them to the tail of this queue.

enqueue(mbuf_t)

Adds a chain of packets to the tail of the queue.

enqueueWithDrop

Adds a chain of packets to the tail of the queue.

flush

Frees all packets currently held in the queue and releases them back to the free mbuf pool.

free

Frees the IOPacketQueue object.

getCapacity

Gets the current capacity of the queue.

getSize

Gets the size of the queue.

initWithCapacity

Initializes an IOPacketQueue object.

lockDequeue

Removes a single packet from the head of a synchronized queue.

lockDequeueAll

Removes all packets from a synchronized queue and returns the head of the packet chain.

lockEnqueue

Adds a chain of packets to the tail of a synchronized queue.

lockEnqueueWithDrop

Adds a chain of packets to the tail of a synchronized queue.

lockFlush

Frees all packets currently held in a synchronized queue and releases them back to the free mbuf pool.

lockPrepend

Adds a chain of packets to the head of a synchronized queue.

peek

Examines the packet at the head of the queue without removing it from the queue.

prepend(IOPacketQueue *)

Removes all packets from the specified queue, and adds them to the head of this queue.

prepend(mbuf_t)

Adds a chain of packets to the head of the queue.

setCapacity

Changes the capacity of the queue.

withCapacity

Factory method that constructs and initializes an IOPacketQueue object.

### Constants

IOPacketQueueDefaultCapacity

Describes the default capacity of the queue object.

### Instance Variables

_reserved

### Instance Methods

- dequeue

- dequeueAll

- enqueue

- enqueue

- enqueueWithDrop

- flush

- free

- getCapacity

- getMetaClass

- getSize

- initWithCapacity

- lockDequeue

- lockDequeueAll

- lockEnqueue

- lockEnqueueWithDrop

- lockFlush

- lockPrepend

- peek

- prepend

- prepend

- setCapacity

### Type Methods

+ withCapacity

## Relationships

### Inherits From

- OSObject

## See Also

### Network Data

IONetworkData

An object that manages a fixed-size named buffer.

IONetworkMedium

An object that encapsulates information about a network medium (i.e. 10Base-T, or 100Base-T Full Duplex).

IOPacketBufferConstraints

