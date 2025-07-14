

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryMap
-  redirect 

# redirect

Replace the memory mapped in a process with new backing memory.

``` source
#ifndef __LP64__
 virtual IOReturn redirect(
 IOMemoryDescriptor *newBackingMemory, 
 IOOptionBits options, 
 IOByteCount offset = 0); 
#endif
```

## Parameters 

`newBackingMemory`  

The IOMemoryDescriptor that represents the physical memory that is to be now mapped in the virtual range the IOMemoryMap represents. If newBackingMemory is NULL, any access to the mapping will hang (in vm_fault()) until access has been restored by a new call to redirect() with non-NULL newBackingMemory argument.

`options`  

Mapping options are defined in IOTypes.h, and are documented in IOMemoryDescriptor::map()

`offset`  

As with IOMemoryDescriptor::map(), a beginning offset into the IOMemoryDescriptor's memory where the mapping starts. Zero is the default.

## Return Value

An IOReturn code.

## Overview

An IOMemoryMap created with the kIOMapUnique option to IOMemoryDescriptor::map() can remapped to a new IOMemoryDescriptor backing object. If the new IOMemoryDescriptor is specified as NULL, client access to the memory map is blocked until a new backing object has been set. By blocking access and copying data, the caller can create atomic copies of the memory while the client is potentially reading or writing the memory.

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

unmap

Force the IOMemoryMap to unmap, without destroying the object.

