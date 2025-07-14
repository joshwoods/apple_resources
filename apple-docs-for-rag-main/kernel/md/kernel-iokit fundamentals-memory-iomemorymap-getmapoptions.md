

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryMap
-  getMapOptions 

# getMapOptions

Accessor to the options the mapping was created with.

``` source
virtual IOOptionBits getMapOptions(); 
```

## Return Value

Options for the mapping, including cache settings.

## Overview

This method returns the options to IOMemoryDescriptor::map the mapping was created with.

## See Also

### Miscellaneous

getAddress()

Accessor to the length of the mapping.

getAddressTask

Accessor to the task of the mapping.

getLength

Accessor to the length of the mapping.

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

unmap

Force the IOMemoryMap to unmap, without destroying the object.

