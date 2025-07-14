

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryMap
-  getPhysicalSegment 

# getPhysicalSegment

Break a mapping into its physically contiguous segments.

``` source
#ifdef __LP64__
 virtual IOPhysicalAddress getPhysicalSegment(
 IOByteCount offset, 
 IOByteCount *length, 
 IOOptionBits options = 0); 
#else /* !__LP64__ */
virtual IOPhysicalAddress getPhysicalSegment(
 IOByteCount offset, 
 IOByteCount *length); 
#endif 
/* !__LP64__ */
```

## Parameters 

`offset`  

A byte offset into the mapping whose physical address to return.

`length`  

If non-zero, getPhysicalSegment will store here the length of the physically contiguous segement at the given offset.

## Return Value

A physical address, or zero if the offset is beyond the length of the mapping.

## Overview

This method returns the physical address of the byte at the given offset into the mapping, and optionally the length of the physically contiguous segment from that offset. It functions similarly to IOMemoryDescriptor::getPhysicalSegment.

## See Also

### Miscellaneous

getAddress()

Accessor to the length of the mapping.

getAddressTask

Accessor to the task of the mapping.

getLength

Accessor to the length of the mapping.

getMapOptions

Accessor to the options the mapping was created with.

getMemoryDescriptor

Accessor to the IOMemoryDescriptor the mapping was created from.

getPhysicalAddress

Return the physical address of the first byte in the mapping.

getSize()

Accessor to the length of the mapping.

getVirtualAddress

Accessor to the virtual address of the first byte in the mapping.

redirect

Replace the memory mapped in a process with new backing memory.

unmap

Force the IOMemoryMap to unmap, without destroying the object.

