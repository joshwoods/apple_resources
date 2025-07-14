

- NetworkingDriverKit
- IOUserNetworkPacket
-  GetDataLength 

Instance Method

# GetDataLength

Gets the number of bytes of data in the packet.

DriverKit

``` source
kern_return_t GetDataLength(uint32_t * length) const;
```

## Parameters 

`length`  

On return, the data length value.

## Return Value

`kIOReturnSuccess` on success, or another value if an error occurred.

## See Also

### Getting the Packet Information

GetHeadroom

Gets the number of bytes reserved at the front of the packet’s buffer.

GetLinkHeaderLength

Gets the number of bytes to use for the link header.

GetDataOffset

Gets the offset to the beginning of the packet’s data.

GetMemorySegmentOffset

Gets the offset to the beginning of the packet in the corresponding memory buffer.

