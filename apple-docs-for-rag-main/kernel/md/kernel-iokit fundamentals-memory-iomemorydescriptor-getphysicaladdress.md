

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryDescriptor
-  getPhysicalAddress 

# getPhysicalAddress

Return the physical address of the first byte in the memory.

``` source
IOPhysicalAddress getPhysicalAddress(); 
```

## Return Value

A physical address.

## Overview

This method returns the physical address of the first byte in the memory. It is most useful on memory known to be physically contiguous.

## See Also

### Getting the Memory Pages

getPageCounts

Retrieve the number of resident and/or dirty pages encompassed by a memory descriptor.

- getPageCounts

Retrieve the number of resident and/or dirty pages encompassed by a memory descriptor.

- getPhysicalAddress

Return the physical address of the first byte in the memory.

getPhysicalSegment

Break a memory descriptor into its physically contiguous segments.

- getPhysicalSegment

Break a memory descriptor into its physically contiguous segments.

