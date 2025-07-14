

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOOutputQueue
-  getMbufPriority 

# getMbufPriority

Determines an mbuf's traffic priority. The highest priority is 0.

``` source
virtual UInt32 getMbufPriority(
 mbuf_tm); 
```

## Parameters 

`m`  

An mbuf to analyze.

## Return Value

Returns a UInt32 representing the priority of the packet. 0 is the highest priority.

## Overview

A queue can prioritize certain classes of traffic. This method facilitates that by evaluating an mbuf and returning its priority.

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

