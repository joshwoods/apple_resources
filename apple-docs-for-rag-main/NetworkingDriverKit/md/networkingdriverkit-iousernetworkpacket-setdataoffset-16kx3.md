

- NetworkingDriverKit
- IOUserNetworkPacket
-  SetDataOffset 

Instance Method

# SetDataOffset

Changes the offset to the beginning of the packet’s data to the specified value.

DriverKit

``` source
kern_return_t SetDataOffset(uint16_t offset);
```

## Parameters 

`offset`  

The new data offset value, specified in bytes from the beginning of the buffer.

## Return Value

`kIOReturnSuccess` on success, or another value if an error occurred.

## See Also

### Configuring the Packet State Information

SetHeadroom

Changes the number of bytes to reserve at the front of the packet’s buffer to the specified value.

SetLinkHeaderLength

Changes the number of bytes to use for the link header to the specified value.

SetDataLength

Changes the number of bytes of data in the packet to the specified value.

