

- NetworkingDriverKit
-  IOUserNetworkRxCompletionQueue 

Class

# IOUserNetworkRxCompletionQueue

The queue you use to store packets that you successfully transferred to the networking stack.

DriverKit

``` source
class IOUserNetworkRxCompletionQueue;
```

## Overview

Create an IOUserNetworkRxCompletionQueue object and use it to deliver packets from your hardware device to the networking stack. As data arrives from your hardware, place the data into empty packets that you dequeued from an IOUserNetworkRxSubmissionQueue object. Deliver the resulting packets to the system by enqueueing them on your IOUserNetworkRxCompletionQueue object. After you enqueue the packets, the system transfers the packet data to the networking stack, recycles the packets, and places the packets back in your submission queue.

## Topics

### Creating the Completion Queue

Create

Creates a queue that you use to deliver packets received from your hardware device.

init

Initializes the packet submission queue.

free

Performs any final cleanup for the queue.

### Instance Methods

initWithPool

setPacketPoller

### Type Methods

withPool

## Relationships

### Inherits From

- IOUserNetworkPacketQueue

## See Also

### Packet Queues

IOUserNetworkRxSubmissionQueue

The queue that receives packets from the device.

IOUserNetworkTxSubmissionQueue

The queue that receives packets from the networking stack.

IOUserNetworkTxCompletionQueue

The queue you use to store packets that you successfully transferred to the device.

IOUserNetworkPacketQueue

The base class for the queues that manage the packets moving to and from your device.

