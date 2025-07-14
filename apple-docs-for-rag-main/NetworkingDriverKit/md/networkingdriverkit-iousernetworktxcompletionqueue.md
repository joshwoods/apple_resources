

- NetworkingDriverKit
-  IOUserNetworkTxCompletionQueue 

Class

# IOUserNetworkTxCompletionQueue

The queue you use to store packets that you successfully transferred to the device.

DriverKit

``` source
class IOUserNetworkTxCompletionQueue;
```

## Overview

Create an IOUserNetworkTxCompletionQueue object and use it to return packets back to the system after sending them to your hardware. The system recycles the packets you place on this queue, reusing them for new packets that it places in your IOUserNetworkTxSubmissionQueue.

## Topics

### Creating the Completion Queue

Create

Creates a queue that tells the system which packets you transmitted to your device.

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

IOUserNetworkRxCompletionQueue

The queue you use to store packets that you successfully transferred to the networking stack.

IOUserNetworkTxSubmissionQueue

The queue that receives packets from the networking stack.

IOUserNetworkPacketQueue

The base class for the queues that manage the packets moving to and from your device.

