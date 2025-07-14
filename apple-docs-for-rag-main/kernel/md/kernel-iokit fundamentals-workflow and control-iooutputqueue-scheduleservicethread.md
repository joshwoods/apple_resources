

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOOutputQueue
-  scheduleServiceThread 

# scheduleServiceThread

Schedules a service thread callout.

``` source
virtual bool scheduleServiceThread(
 void *param = 0); 
```

## Parameters 

`param`  

A parameter to pass to the serviceThread() method.

## Return Value

Returns true if a thread callout was scheduled, false otherwise.

## Overview

This method can be called by service() to schedule a thread that will call serviceThread() when it starts running.

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

