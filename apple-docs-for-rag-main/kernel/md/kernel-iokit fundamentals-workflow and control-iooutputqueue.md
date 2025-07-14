

- Kernel
- IOKit Fundamentals
- Workflow and Control
-  IOOutputQueue 

Class

# IOOutputQueue

A packet queue that supports multiple producers and a single consumer.

macOS 10.0+

``` source
class IOOutputQueue : OSObject
```

## Overview

Each producer, or a client thread, will deliver a chain of packets to the queue. A single consumer will remove packets from the queue one at a time and forward it to the registered target/action. This object may be used by an IONetworkController on the output (transmit) side to handle the output packet flow downstream from an IONetworkInterface, and then call the driver's output function. IOOutputQueue is an abstract class that provides an interface for its subclasses. Concrete subclasses will complete the implementation, and specify the context that the target is called for packets removed from the queue.

## Topics

### Miscellaneous

cancelServiceThread

Cancels any pending service thread callout.

enqueue

Adds a packet, or a chain of packets, to the queue.

flush

Drops and frees all packets currently held by the queue.

free

Frees the IOOutputQueue object.

getCapacity

Gets the number of packets that the queue can hold.

getMbufPriority

Determines an mbuf's traffic priority. The highest priority is 0.

getOutputHandler

Returns the address of a function that is designated to handle incoming packets sent to the queue object.

getSize

Gets the number of packets currently held in the queue.

getStatisticsData

Returns an IONetworkData object containing statistics counters updated by the queue.

init

Initializes an IOOutputQueue object.

scheduleServiceThread

Schedules a service thread callout.

service

Services the queue.

serviceThread

Method called by the scheduled service thread when it starts to run.

setCapacity

Changes the number of packets that the queue can hold before it begins to drop excess packets.

start

Starts up the queue.

stop

Stops the queue.

### Instance Variables

_reserved

### Instance Methods

- cancelServiceThread

- enqueue

- flush

- free

- getCapacity

- getMbufPriority

- getMetaClass

- getOutputHandler

- getSize

- getStatisticsData

- init

- scheduleServiceThread

- service

- serviceThread

- setCapacity

- start

- stop

### Type Methods

+ runServiceThread

## Relationships

### Inherits From

- OSObject

## See Also

### Output Queues

IOGatedOutputQueue

An extension of an IOBasicOutputQueue.

IOBasicOutputQueue

A concrete implementation of an IOOutputQueue.

