

- Kernel
- IOKit Fundamentals
- Workflow and Control
-  IOBasicOutputQueue 

Class

# IOBasicOutputQueue

A concrete implementation of an IOOutputQueue.

macOS 10.0+

``` source
class IOBasicOutputQueue : IOOutputQueue
```

## Overview

This object uses a mutex to protect the packet queue from multiple producers. A single producer is promoted to become a consumer when the queue is not active. Otherwise, the producer will simply queue the packet and return without blocking.

The flow of packets from the queue to its target can be controlled by calling methods such as start(), stop(), or service(). The target is expected to call those methods from a single threaded context, i.e. the work loop context in a network driver. In addition, the target must also return a status for every packet delivered by the consumer thread. This return value is the only mechanism that the target can use to manage the queue when it is running on the consumer thread.

## Topics

### Miscellaneous

enqueue

Adds a packet, or a chain of packets, to the queue.

flush

Drops and frees all packets currently held by the queue.

free

Frees the IOBasicOutputQueue object.

getCapacity

Gets the number of packets that the queue can hold.

getDropCount

Gets the number of packets dropped by the queue.

getOutputCount

Gets the number of packets accepted by the target.

getRetryCount

Gets the number of instances when the target has refused to accept the packet provided.

getSize

Gets the number of packets currently held in the queue.

getStallCount

Gets the number of instances when the target has stalled the queue.

getState

Gets the state of the queue object.

getStatisticsData

Returns an IONetworkData object containing statistics counters updated by the queue.

handleNetworkDataAccess

Handles an external access to the IONetworkData object returned by getStatisticsData().

init

Initializes an IOBasicOutputQueue object.

output

Transfers all packets in the mbuf queue to the target.

service

Services a queue that was stalled by the target.

serviceThread

Provides an implementation for the serviceThread() method defined in IOOutputQueue.

setCapacity

Changes the number of packets that the queue can hold before it begins to drop excess packets.

start

Starts up the packet flow between the queue and its target.

stop

Stops the packet flow between the queue and its target.

withTarget(IONetworkController *, UInt32)

Factory method that constructs and initializes an IOBasicOutputQueue object.

withTarget(IONetworkController *, UInt32, UInt32)

Factory method that constructs and initializes an IOBasicOutputQueue object.

withTarget(OSObject *, IOOutputAction, UInt32)

Factory method that constructs and initializes an IOBasicOutputQueue object.

withTarget(OSObject *, IOOutputAction, UInt32, UInt32)

Factory method that constructs and initializes an IOBasicOutputQueue object.

### Constants

GetStateBits

The bits in the value returned by getState().

ServiceAsync

The option bits recognized by service().

### Instance Methods

- dequeue

- enqueue

- flush

- free

- getCapacity

- getDropCount

- getMetaClass

- getOutputCount

- getRetryCount

- getSize

- getStallCount

- getState

- getStatisticsData

- handleNetworkDataAccess

- output

- service

- serviceThread

- setCapacity

- start

- stop

### Type Methods

+ dispatchNetworkDataNotification

+ withTarget

+ withTarget

## Relationships

### Inherits From

- IOOutputQueue

## See Also

### Output Queues

IOGatedOutputQueue

An extension of an IOBasicOutputQueue.

IOOutputQueue

A packet queue that supports multiple producers and a single consumer.

