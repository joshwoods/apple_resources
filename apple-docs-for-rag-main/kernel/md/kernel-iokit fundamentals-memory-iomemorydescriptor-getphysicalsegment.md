

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryDescriptor
-  getPhysicalSegment 

# getPhysicalSegment

Break a memory descriptor into its physically contiguous segments.

``` source
#ifdef __LP64__
 virtual addr64_t getPhysicalSegment(
 IOByteCount offset, 
 IOByteCount *length, 
 IOOptionBits options = 0 ) = 0; 
#else /* !__LP64__ */
virtual addr64_t getPhysicalSegment(
 IOByteCount offset, 
 IOByteCount *length, 
 IOOptionBits options ); 
#endif 
/* !__LP64__ */
```

## Parameters 

`offset`  

A byte offset into the memory whose physical address to return.

`length`  

If non-zero, getPhysicalSegment will store here the length of the physically contiguous segement at the given offset.

`options`  

Additional options.

## Return Value

A physical address, or zero if the offset is beyond the length of the memory.

## Overview

This method returns the physical address of the byte at the given offset into the memory, and optionally the length of the physically contiguous segment from that offset.

## See Also

### Getting the Memory Pages

getPageCounts

Retrieve the number of resident and/or dirty pages encompassed by a memory descriptor.

- getPageCounts

Retrieve the number of resident and/or dirty pages encompassed by a memory descriptor.

getPhysicalAddress

Return the physical address of the first byte in the memory.

- getPhysicalAddress

Return the physical address of the first byte in the memory.

- getPhysicalSegment

Break a memory descriptor into its physically contiguous segments.

