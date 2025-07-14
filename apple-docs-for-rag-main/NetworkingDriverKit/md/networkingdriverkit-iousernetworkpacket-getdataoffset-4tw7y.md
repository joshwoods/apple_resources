

- NetworkingDriverKit
- IOUserNetworkPacket
-  GetDataOffset 

Instance Method

# GetDataOffset

Gets the offset to the beginning of the packet’s data.

DriverKit

``` source
kern_return_t GetDataOffset(uint16_t * offset) const;
```

## Parameters 

`offset`  

On return, the offset value.

## Return Value

`kIOReturnSuccess` on success, or another value if an error occurred.

## See Also

### Getting the Packet Information

GetHeadroom

Gets the number of bytes reserved at the front of the packet’s buffer.

GetLinkHeaderLength

Gets the number of bytes to use for the link header.

GetDataLength

Gets the number of bytes of data in the packet.

GetMemorySegmentOffset

Gets the offset to the beginning of the packet in the corresponding memory buffer.

