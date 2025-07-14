

- Kernel
- Hardware Families
- Network
- IOPacketQueue
-  enqueue(mbuf_t) 

# enqueue(mbuf_t)

Adds a chain of packets to the tail of the queue.

``` source
virtual bool enqueue(
 mbuf_tm); 
```

## Parameters 

`m`  

A chain of packets to add to the tail of the queue.

## Return Value

Returns true on success, or false to indicate over-capacity and refusal to accept the packet chain provided.

## Overview

Packets are not added if the size of the queue has reached its capacity.

## See Also

### Miscellaneous

dequeue

Removes a single packet from the head of the queue.

dequeueAll

Removes all packets from the queue and returns the head of the packet chain.

enqueue(IOPacketQueue *)

Removes all packets from the specified queue, and adds them to the tail of this queue.

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

