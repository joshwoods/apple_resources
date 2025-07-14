

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOOutputQueue
-  setCapacity 

# setCapacity

Changes the number of packets that the queue can hold before it begins to drop excess packets.

``` source
virtual bool setCapacity(
 UInt32capacity) = 0; 
```

## Parameters 

`capacity`  

The new desired capacity.

## Return Value

Returns true if the new capacity was accepted, false otherwise.

## See Also

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

start

Starts up the queue.

stop

Stops the queue.

