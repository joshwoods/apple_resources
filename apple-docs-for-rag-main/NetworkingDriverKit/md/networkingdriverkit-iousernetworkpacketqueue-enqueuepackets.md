

- NetworkingDriverKit
- IOUserNetworkPacketQueue
-  EnqueuePackets 

Instance Method

# EnqueuePackets

Adds multiple network packets to the queue for processing.

DriverKit

``` source
uint32_t EnqueuePackets(IOUserNetworkPacket * * packets, uint32_t packetCount);
```

## Parameters 

`packets`  

An array of network packets you want to add to the queue.

`packetCount`  

The number of network packets in the `packets` parameter.

## Return Value

The number of packets actually added to the queue.

## Discussion

Call this method when you are ready to submit multiple packets to a completion queue for processing. After the system processes the enqueued network packets, it recycles them and makes them available on the corresponding submission queue.

## See Also

### Queueing and Dequeueing Packets

EnqueuePacket

Adds a single network packet to the queue for processing.

DequeuePacket

Retrieves a single network packet from the queue.

DequeuePackets

Retrieves multiple network packets from the queue.

