

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryMap
-  getMemoryDescriptor 

# getMemoryDescriptor

Accessor to the IOMemoryDescriptor the mapping was created from.

``` source
virtual IOMemoryDescriptor * getMemoryDescriptor(); 
```

## Return Value

An IOMemoryDescriptor reference, which is valid while the IOMemoryMap object is retained. It should not be released by the caller.

## Overview

This method returns the IOMemoryDescriptor the mapping was created from.

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

getPhysicalAddress

Return the physical address of the first byte in the mapping.

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

