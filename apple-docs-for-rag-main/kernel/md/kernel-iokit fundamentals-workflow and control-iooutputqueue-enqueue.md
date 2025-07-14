

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOOutputQueue
-  enqueue 

# enqueue

Adds a packet, or a chain of packets, to the queue.

``` source
virtual UInt32 enqueue(
 mbuf_tm,
 void *param) = 0; 
```

## Parameters 

`m`  

A single packet, or a chain of packets.

`param`  

A parameter provided by the caller.

## Return Value

Returns a return code.

## Overview

This method is called by a client to add a packet, or a chain of packets, to the queue. A packet is described by an mbuf chain, while a chain of packets is constructed by linking multiple mbuf chains via the m_nextpkt field.

## See Also

### Miscellaneous

cancelServiceThread

Cancels any pending service thread callout.

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

