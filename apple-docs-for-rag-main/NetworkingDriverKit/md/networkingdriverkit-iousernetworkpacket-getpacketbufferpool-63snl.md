

- NetworkingDriverKit
- IOUserNetworkPacket
-  GetPacketBufferPool 

Instance Method

# GetPacketBufferPool

Gets the memory buffer that contains the pakcet.

DriverKit

``` source
kern_return_t GetPacketBufferPool(IOUserNetworkPacketBufferPool * * pool) const;
```

## Parameters 

`pool`  

On return, the memory buffer containing the packet.

## Return Value

`kIOReturnSuccess` on success, or another value if an error occurred.

