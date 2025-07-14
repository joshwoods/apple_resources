

- Kernel
- IOKit Fundamentals
- Memory
- IODMACommand
-  readBytes 

# readBytes

Copy data from the IODMACommand's buffer to the specified buffer.

``` source
UInt64 readBytes(
 UInt64offset,
 void *bytes,
 UInt64length); 
```

## Parameters 

`offset`  

A byte offset into the IODMACommand's memory, relative to the prepared offset.

`bytes`  

The caller supplied buffer to copy the data to.

`length`  

The length of the data to copy.

## Return Value

The number of bytes copied, zero will be returned if the specified offset is beyond the prepared length of the IODMACommand.

## Overview

This method copies data from the IODMACommand's memory at the given offset, to the caller's buffer. The IODMACommand must be prepared, and the offset is relative to the prepared offset.

## See Also

### Transferring Data

- readBytes

Copy data from the IODMACommand's buffer to the specified buffer.

writeBytes

Copy data to the IODMACommand's buffer from the specified buffer.

- writeBytes

Copy data to the IODMACommand's buffer from the specified buffer.

