

- NetworkingDriverKit
- IOUserNetworkPacket
-  GetHeadroom 

Instance Method

# GetHeadroom

Gets the number of bytes reserved at the front of the packet’s buffer.

DriverKit

``` source
kern_return_t GetHeadroom(uint8_t * headroom) const;
```

## Parameters 

`headroom`  

On return, the headroom value.

## Return Value

`kIOReturnSuccess` on success, or another value if an error occurred.

## See Also

### Getting the Packet Information

GetLinkHeaderLength

Gets the number of bytes to use for the link header.

GetDataOffset

Gets the offset to the beginning of the packet’s data.

GetDataLength

Gets the number of bytes of data in the packet.

GetMemorySegmentOffset

Gets the offset to the beginning of the packet in the corresponding memory buffer.

