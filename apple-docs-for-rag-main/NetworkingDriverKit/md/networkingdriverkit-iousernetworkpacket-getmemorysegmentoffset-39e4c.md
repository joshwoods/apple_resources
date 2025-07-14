

- NetworkingDriverKit
- IOUserNetworkPacket
-  GetMemorySegmentOffset 

Instance Method

# GetMemorySegmentOffset

Gets the offset to the beginning of the packet in the corresponding memory buffer.

DriverKit

``` source
kern_return_t GetMemorySegmentOffset(uint64_t * offset) const;
```

## Parameters 

`offset`  

On return, the memory segment offset value.

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

GetDataLength

Gets the number of bytes of data in the packet.

