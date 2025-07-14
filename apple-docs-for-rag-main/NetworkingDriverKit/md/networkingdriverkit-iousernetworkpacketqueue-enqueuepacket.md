

- NetworkingDriverKit
- IOUserNetworkPacketQueue
-  EnqueuePacket 

Instance Method

# EnqueuePacket

Adds a single network packet to the queue for processing.

DriverKit

``` source
kern_return_t EnqueuePacket(IOUserNetworkPacket * packet);
```

## Parameters 

`packet`  

The packet to add to the queue.

## Return Value

`kIOReturnSuccess` on success, or another value if an error occurred.

## Discussion

Call this method when you are ready to submit a single packet to a completion queue for processing. After the system processes the enqueued network packet, it recycles it and makes it available on the corresponding submission queue.

## See Also

### Queueing and Dequeueing Packets

EnqueuePackets

Adds multiple network packets to the queue for processing.

DequeuePacket

Retrieves a single network packet from the queue.

DequeuePackets

Retrieves multiple network packets from the queue.

