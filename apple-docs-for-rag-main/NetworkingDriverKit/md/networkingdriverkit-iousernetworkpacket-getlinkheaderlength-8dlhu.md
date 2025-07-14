

- NetworkingDriverKit
- IOUserNetworkPacket
-  GetLinkHeaderLength 

Instance Method

# GetLinkHeaderLength

Gets the number of bytes to use for the link header.

DriverKit

``` source
kern_return_t GetLinkHeaderLength(uint8_t * length) const;
```

## Parameters 

`length`  

On return, the link header length value.

## Return Value

`kIOReturnSuccess` on success, or another value if an error occurred.

## See Also

### Getting the Packet Information

GetHeadroom

Gets the number of bytes reserved at the front of the packet’s buffer.

GetDataOffset

Gets the offset to the beginning of the packet’s data.

GetDataLength

Gets the number of bytes of data in the packet.

GetMemorySegmentOffset

Gets the offset to the beginning of the packet in the corresponding memory buffer.

