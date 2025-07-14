

- NetworkingDriverKit
- IOUserNetworkPacketBufferPool
-  DeallocatePacket 

Instance Method

# DeallocatePacket

Disposes of any resources associated with the packet and makes the packet available for reuse.

DriverKit

``` source
kern_return_t DeallocatePacket(IOUserNetworkPacket * packet);
```

## Parameters 

`packet`  

The packet to deallocate. It is a programmer error to specify `NULL` or an invalid pointer for this parameter.

## Return Value

`kIOReturnSuccess` on success, or another value if an error occurred.

## Discussion

After you move a packet to the appropriate completion queue, call this method to recycle the packet. Recycling the packet makes it available for use with a new incoming or outgoing packet.

## See Also

### Deallocating Packets

DeallocatePackets

Disposes of any resources associated with the specified packets and makes them available for reuse.

