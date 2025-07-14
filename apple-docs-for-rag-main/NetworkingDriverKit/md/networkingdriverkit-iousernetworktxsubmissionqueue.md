

- NetworkingDriverKit
-  IOUserNetworkTxSubmissionQueue 

Class

# IOUserNetworkTxSubmissionQueue

The queue that receives packets from the networking stack.

DriverKit

``` source
class IOUserNetworkTxSubmissionQueue;
```

## Overview

Create an IOUserNetworkTxSubmissionQueue in your driver and use it to dequeue empty packets. As your driver receives data from the networking stack, fill the empty packets with data send them to your hardware device. After sending the packets, enqueue them on your IOUserNetworkTxCompletionQueue object so that the system can reclaim them and make them available for reuse later.

## Topics

### Creating the Submission Queue

init

Initializes the packet submission queue.

free

Performs any final cleanup for the queue.

### Instance Methods

initWithPool

purgePackets

### Type Methods

Create

Create

withPool

withPoolAndServiceClass

## Relationships

### Inherits From

- IOUserNetworkPacketQueue

## See Also

### Packet Queues

IOUserNetworkRxSubmissionQueue

The queue that receives packets from the device.

IOUserNetworkRxCompletionQueue

The queue you use to store packets that you successfully transferred to the networking stack.

IOUserNetworkTxCompletionQueue

The queue you use to store packets that you successfully transferred to the device.

IOUserNetworkPacketQueue

The base class for the queues that manage the packets moving to and from your device.

