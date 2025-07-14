

- DriverKit
-  IOAddressSegment 

Structure

# IOAddressSegment

A structure that describes the location and size of a block of memory.

DriverKitiOSiPadOSmacOS

``` source
struct IOAddressSegment;
```

## Topics

### Getting the Address Information

address

The address of the buffer in the current process’ virtual memory space.

length

The size of the memory buffer, in bytes.

## See Also

### Managing the Buffer Contents

SetLength

Changes the length of the memory buffer.

GetAddressRange

Returns the address and length of the memory buffer.

