

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOBasicOutputQueue
-  withTarget(IONetworkController \*, UInt32) 

# withTarget(IONetworkController \*, UInt32)

Factory method that constructs and initializes an IOBasicOutputQueue object.

``` source
static IOBasicOutputQueue * withTarget(
 IONetworkController *target, 
 UInt32 capacity = 0); 
```

## Parameters 

`target`  

An IONetworkController object that will handle packets removed from the queue.

`capacity`  

The initial capacity of the output queue.

## Return Value

Returns an IOBasicOutputQueue object on success, or 0 otherwise.

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

withTarget(IONetworkController *, UInt32, UInt32)

Factory method that constructs and initializes an IOBasicOutputQueue object.

withTarget(OSObject *, IOOutputAction, UInt32)

Factory method that constructs and initializes an IOBasicOutputQueue object.

withTarget(OSObject *, IOOutputAction, UInt32, UInt32)

Factory method that constructs and initializes an IOBasicOutputQueue object.

