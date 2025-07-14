

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOOutputQueue
-  start 

# start

Starts up the queue.

``` source
virtual bool start() = 0; 
```

## Return Value

Returns true if the queue was started successfully, false otherwise.

## Overview

This method is called by the target to start the queue. This will allow packets to be removed from the queue, then delivered to the target.

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

setCapacity

Changes the number of packets that the queue can hold before it begins to drop excess packets.

stop

Stops the queue.

