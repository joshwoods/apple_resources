

- Kernel
- IOKit Fundamentals
- Memory
- IODMACommand
-  writeBytes 

# writeBytes

Copy data to the IODMACommand's buffer from the specified buffer.

``` source
UInt64 writeBytes(
 UInt64offset,
 const void *bytes,
 UInt64length); 
```

## Parameters 

`offset`  

A byte offset into the IODMACommand's memory, relative to the prepared offset.

`bytes`  

The caller supplied buffer to copy the data from.

`length`  

The length of the data to copy.

## Return Value

The number of bytes copied, zero will be returned if the specified offset is beyond the prepared length of the IODMACommand.

## Overview

This method copies data to the IODMACommand's memory at the given offset, from the caller's buffer. The IODMACommand must be prepared, and the offset is relative to the prepared offset.

## See Also

### Transferring Data

readBytes

Copy data from the IODMACommand's buffer to the specified buffer.

- readBytes

Copy data from the IODMACommand's buffer to the specified buffer.

- writeBytes

Copy data to the IODMACommand's buffer from the specified buffer.

