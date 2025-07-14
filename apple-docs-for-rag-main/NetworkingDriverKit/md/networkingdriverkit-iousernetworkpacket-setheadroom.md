

- NetworkingDriverKit
- IOUserNetworkPacket
-  SetHeadroom 

Instance Method

# SetHeadroom

Changes the number of bytes to reserve at the front of the packet’s buffer to the specified value.

DriverKit

``` source
kern_return_t SetHeadroom(uint8_t headroom);
```

## Parameters 

`headroom`  

The new headroom value, specified in bytes.

## Return Value

`kIOReturnSuccess` on success, or another value if an error occurred.

## See Also

### Configuring the Packet State Information

SetLinkHeaderLength

Changes the number of bytes to use for the link header to the specified value.

SetDataOffset

Changes the offset to the beginning of the packet’s data to the specified value.

SetDataLength

Changes the number of bytes of data in the packet to the specified value.

