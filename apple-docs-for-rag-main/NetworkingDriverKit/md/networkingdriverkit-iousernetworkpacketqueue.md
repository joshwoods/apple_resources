

- NetworkingDriverKit
-  IOUserNetworkPacketQueue 

Class

# IOUserNetworkPacketQueue

The base class for the queues that manage the packets moving to and from your device.

DriverKit

``` source
class IOUserNetworkPacketQueue;
```

## Overview

This class provides the common functionality for the submission and completion queues you use to manage network packets. You do not create instances of this class directly. Instead, you instantiate the following concrete subclasses:

- IOUserNetworkRxSubmissionQueue

- IOUserNetworkRxCompletionQueue

- IOUserNetworkTxSubmissionQueue

- IOUserNetworkTxCompletionQueue

Submission queues contain the packets that your driver dequeues and processes. After you process the dequeued packets, you place them on the matching completion queue to let the system know that you are finished with them. The system eventually recycles the completed packets back to the corresponding submission queue so that the cycle may begin again.

## Topics

### Configuring the Packet Queue

init

Initializes the packet submission queue.

free

Performs any final cleanup for the queue.

### Enabling the Packet Queue

SetEnable

Enables or disables the queue.

### Queueing and Dequeueing Packets

EnqueuePacket

Adds a single network packet to the queue for processing.

EnqueuePackets

Adds multiple network packets to the queue for processing.

DequeuePacket

Retrieves a single network packet from the queue.

DequeuePackets

Retrieves multiple network packets from the queue.

### Configuring the Queue Attributes

SetPacketBufferPool

Assigns the specified buffer pool with this queue.

SetPacketDirection

Specifies whether packets flow into or out of the queue.

### Managing the Data Queue

CopyDataQueue

Returns the dispatch queue that this object uses to execute tasks.

SetDataQueue

Assigns the specified dispatch source to this object.

### Instance Methods

enqueuePackets

requestDequeue

requestEnqueue

setEnable

setPacketPoller

## Relationships

### Inherits From

- OSObject

### Inherited By

- IOUserNetworkRxCompletionQueue
- IOUserNetworkRxSubmissionQueue
- IOUserNetworkTxCompletionQueue
- IOUserNetworkTxSubmissionQueue

## See Also

### Packet Queues

IOUserNetworkRxSubmissionQueue

The queue that receives packets from the device.

IOUserNetworkRxCompletionQueue

The queue you use to store packets that you successfully transferred to the networking stack.

IOUserNetworkTxSubmissionQueue

The queue that receives packets from the networking stack.

IOUserNetworkTxCompletionQueue

The queue you use to store packets that you successfully transferred to the device.

