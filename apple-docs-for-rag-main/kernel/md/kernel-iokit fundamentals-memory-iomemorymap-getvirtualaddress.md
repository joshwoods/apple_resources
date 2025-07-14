

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryMap
-  getVirtualAddress 

# getVirtualAddress

Accessor to the virtual address of the first byte in the mapping.

``` source
virtual IOVirtualAddress getVirtualAddress(); 
```

## Return Value

A virtual address.

## Overview

This method returns the virtual address of the first byte in the mapping. Since the IOVirtualAddress is only 32bit in 32bit kernels, the getAddress() method should be used for compatibility with 64bit task mappings.

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

redirect

Replace the memory mapped in a process with new backing memory.

unmap

Force the IOMemoryMap to unmap, without destroying the object.

