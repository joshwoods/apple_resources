

- Kernel
- IOKit Fundamentals
- Memory
- IOInterleavedMemoryDescriptor
-  getPhysicalSegment 

# getPhysicalSegment

Break a memory descriptor into its physically contiguous segments.

``` source
virtual addr64_t getPhysicalSegment(
 IOByteCountoffset, 
 IOByteCount *length, 
 IOOptionBits options = 0 ); 
```

## Parameters 

`offset`  

A byte offset into the memory whose physical address to return.

`length`  

If non-zero, getPhysicalSegment will store here the length of the physically contiguous segement at the given offset.

## Return Value

A physical address, or zero if the offset is beyond the length of the memory.

## Overview

This method returns the physical address of the byte at the given offset into the memory, and optionally the length of the physically contiguous segment from that offset.

## See Also

### Miscellaneous

clearMemoryDescriptors

Clear all of the IOMemoryDescriptors currently contained in and reset the IOInterleavedMemoryDescriptor.

complete

Complete processing of the memory after an I/O transfer finishes.

initWithCapacity

Initialize an IOInterleavedMemoryDescriptor to describe a memory area made up of several other IOMemoryDescriptors.

prepare

Prepare the memory for an I/O transfer.

setMemoryDescriptor

Add a portion of an IOMemoryDescriptor to the IOInterleavedMemoryDescriptor.

withCapacity

Create an IOInterleavedMemoryDescriptor to describe a memory area made up of several other IOMemoryDescriptors.

