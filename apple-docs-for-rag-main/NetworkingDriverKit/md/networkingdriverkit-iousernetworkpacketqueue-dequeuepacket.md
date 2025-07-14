

- NetworkingDriverKit
- IOUserNetworkPacketQueue
-  DequeuePacket 

Instance Method

# DequeuePacket

Retrieves a single network packet from the queue.

DriverKit

``` source
kern_return_t DequeuePacket(IOUserNetworkPacket * * packet);
```

## Parameters 

`packet`  

On return, an array containing one element, which represents the next available packet.

## Return Value

`kIOReturnSuccess` on success, or another value if an error occurred.

## Discussion

Call this method to retrieve a single packet from a submission queue. This method returns the requested packet, or an error if no more packets are available.

## See Also

### Queueing and Dequeueing Packets

EnqueuePacket

Adds a single network packet to the queue for processing.

EnqueuePackets

Adds multiple network packets to the queue for processing.

DequeuePackets

Retrieves multiple network packets from the queue.

