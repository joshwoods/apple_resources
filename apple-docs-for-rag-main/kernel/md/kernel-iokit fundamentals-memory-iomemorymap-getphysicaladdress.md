

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryMap
-  getPhysicalAddress 

# getPhysicalAddress

Return the physical address of the first byte in the mapping.

``` source
IOPhysicalAddress getPhysicalAddress(); 
```

## Return Value

A physical address.

## Overview

This method returns the physical address of the first byte in the mapping. It is most useful on mappings known to be physically contiguous.

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

getPhysicalSegment

Break a mapping into its physically contiguous segments.

getSize()

Accessor to the length of the mapping.

getVirtualAddress

Accessor to the virtual address of the first byte in the mapping.

redirect

Replace the memory mapped in a process with new backing memory.

unmap

Force the IOMemoryMap to unmap, without destroying the object.

