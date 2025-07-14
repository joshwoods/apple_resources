

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryMap
-  unmap 

# unmap

Force the IOMemoryMap to unmap, without destroying the object.

``` source
virtual IOReturn unmap(); 
```

## Return Value

An IOReturn code.

## Overview

IOMemoryMap instances will unmap themselves upon free, ie. when the last client with a reference calls release. This method forces the IOMemoryMap to destroy the mapping it represents, regardless of the number of clients. It is not generally used.

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

getPhysicalSegment

Break a mapping into its physically contiguous segments.

getSize()

Accessor to the length of the mapping.

getVirtualAddress

Accessor to the virtual address of the first byte in the mapping.

redirect

Replace the memory mapped in a process with new backing memory.

