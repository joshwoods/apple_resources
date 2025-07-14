

- NetworkingDriverKit
-  IOUserNetworkRxSubmissionQueue 

Class

# IOUserNetworkRxSubmissionQueue

The queue that receives packets from the device.

DriverKit

``` source
class IOUserNetworkRxSubmissionQueue;
```

## Overview

Create an IOUserNetworkRxSubmissionQueue in your driver and use it to dequeue empty packets. As data arrives from your hardware, fill those empty packets with the data. Once the packets are filled, enqueue them on your IOUserNetworkRxCompletionQueue object.

## Topics

### Creating the Submission Queue

Create

Creates a queue that delivers empty packets for you to fill with data from your hardware device.

init

Initializes the packet submission queue.

free

Performs any final cleanup for the queue.

### Instance Methods

initWithPool

### Type Methods

withPool

## Relationships

### Inherits From

- IOUserNetworkPacketQueue

## See Also

### Packet Queues

IOUserNetworkRxCompletionQueue

The queue you use to store packets that you successfully transferred to the networking stack.

IOUserNetworkTxSubmissionQueue

The queue that receives packets from the networking stack.

IOUserNetworkTxCompletionQueue

The queue you use to store packets that you successfully transferred to the device.

IOUserNetworkPacketQueue

The base class for the queues that manage the packets moving to and from your device.

