

- DriverKit
- IOBufferMemoryDescriptor
-  SetLength 

Instance Method

# SetLength

Changes the length of the memory buffer.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t SetLength(uint64_t length);
```

## Parameters 

`length`  

The new length of the memory buffer. This value must be less than or equal to the buffer’s capacity.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

Use this method to truncate an existing memory buffer. For example, you might call this method when repurposing an existing buffer for a new data type. The maximum capacity of the buffer remains unchanged, but the effective length of the buffer changes to the value you specify.

## See Also

### Managing the Buffer Contents

GetAddressRange

Returns the address and length of the memory buffer.

IOAddressSegment

A structure that describes the location and size of a block of memory.

