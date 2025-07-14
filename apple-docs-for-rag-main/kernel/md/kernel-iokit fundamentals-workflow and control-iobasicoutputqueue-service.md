

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOBasicOutputQueue
-  service 

# service

Services a queue that was stalled by the target.

``` source
virtual bool service(
 IOOptionBits options = 0); 
```

## Return Value

Returns true if the queue was stalled and there were packets sitting in the queue awaiting delivery, false otherwise.

## Overview

A target that stalls the queue must call service() when it becomes ready to accept more packets. Calling this method when the queue is not stalled is harmless.

## See Also

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

