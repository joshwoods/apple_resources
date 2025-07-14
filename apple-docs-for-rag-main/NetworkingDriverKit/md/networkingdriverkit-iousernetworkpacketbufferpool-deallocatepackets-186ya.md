

- NetworkingDriverKit
- IOUserNetworkPacketBufferPool
-  DeallocatePackets 

Instance Method

# DeallocatePackets

Disposes of any resources associated with the specified packets and makes them available for reuse.

DriverKit

``` source
kern_return_t DeallocatePackets(IOUserNetworkPacket * * packets, uint32_t packetsCount);
```

## Parameters 

`packets`  

An array of packets to deallocate. It is a programmer error to specify `NULL` or an invalid pointer for this parameter.

`packetsCount`  

The number of items in the `packets` parameter.

## Return Value

`kIOReturnSuccess` on success, or another value if an error occurred.

## Discussion

After you move one or more packets to the appropriate completion queue, call this method to recycle those packets. Recycling packets makes them available for use with new incoming or outgoing packets.

## See Also

### Deallocating Packets

DeallocatePacket

Disposes of any resources associated with the packet and makes the packet available for reuse.

