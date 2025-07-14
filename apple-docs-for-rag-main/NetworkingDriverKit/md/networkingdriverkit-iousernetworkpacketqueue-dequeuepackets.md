

- NetworkingDriverKit
- IOUserNetworkPacketQueue
-  DequeuePackets 

Instance Method

# DequeuePackets

Retrieves multiple network packets from the queue.

DriverKit

``` source
uint32_t DequeuePackets(IOUserNetworkPacket * * packets, uint32_t maxDequeueCount);
```

## Parameters 

`packets`  

On return, an array containing the next available packets.

`maxDequeueCount`  

The number of packets you want to dequeue.

## Return Value

The actual number of packets returned in the `packets` parameter.

## Discussion

Call this method to retrieve multiple packets from the submission queue. This method returns as many packets as are available, up to the maximum number you specify.

## See Also

### Queueing and Dequeueing Packets

EnqueuePacket

Adds a single network packet to the queue for processing.

EnqueuePackets

Adds multiple network packets to the queue for processing.

DequeuePacket

Retrieves a single network packet from the queue.

