

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryDescriptor
-  getPageCounts 

# getPageCounts

Retrieve the number of resident and/or dirty pages encompassed by a memory descriptor.

``` source
IOReturn getPageCounts(
 IOByteCount *residentPageCount, 
 IOByteCount *dirtyPageCount); 
```

## Parameters 

`residentPageCount`  

\- If non-null, a pointer to a byte count that will return the number of resident pages encompassed by this IOMemoryDescriptor.

`dirtyPageCount`  

\- If non-null, a pointer to a byte count that will return the number of dirty pages encompassed by this IOMemoryDescriptor.

## Return Value

An IOReturn code.

## Overview

This method returns the number of resident and/or dirty pages encompassed by an IOMemoryDescriptor.

## See Also

### Getting the Memory Pages

- getPageCounts

Retrieve the number of resident and/or dirty pages encompassed by a memory descriptor.

getPhysicalAddress

Return the physical address of the first byte in the memory.

- getPhysicalAddress

Return the physical address of the first byte in the memory.

getPhysicalSegment

Break a memory descriptor into its physically contiguous segments.

- getPhysicalSegment

Break a memory descriptor into its physically contiguous segments.

