

- DriverKit
- IOBufferMemoryDescriptor
-  GetAddressRange 

Instance Method

# GetAddressRange

Returns the address and length of the memory buffer.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t GetAddressRange(IOAddressSegment * range);
```

## Parameters 

`range`  

An IOAddressSegment structure that you provide. On return, this structure contains the address and length of the memory buffer.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## See Also

### Managing the Buffer Contents

SetLength

Changes the length of the memory buffer.

IOAddressSegment

A structure that describes the location and size of a block of memory.

