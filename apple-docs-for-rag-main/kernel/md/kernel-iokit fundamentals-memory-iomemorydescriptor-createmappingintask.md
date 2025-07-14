

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryDescriptor
-  createMappingInTask 

# createMappingInTask

Maps an IOMemoryDescriptor into a task.

``` source
IOMemoryMap * createMappingInTask( 
 task_t intoTask, 
 mach_vm_address_t atAddress, 
 IOOptionBits options, 
 mach_vm_size_t offset = 0, 
 mach_vm_size_t length = 0 ); 
```

## Parameters 

`intoTask`  

Sets the target task for the mapping. Pass kernel_task for the kernel address space.

`atAddress`  

If a placed mapping is requested, atAddress specifies its address, and the kIOMapAnywhere should not be set. Otherwise, atAddress is ignored.

`options`  

Mapping options are defined in IOTypes.h,

kIOMapAnywhere should be passed if the mapping can be created anywhere. If not set, the atAddress parameter sets the location of the mapping, if it is available in the target map.

kIOMapDefaultCache to inhibit the cache in I/O areas, kIOMapCopybackCache in general purpose RAM.

kIOMapInhibitCache, kIOMapWriteThruCache, kIOMapCopybackCache to set the appropriate caching.

kIOMapReadOnly to allow only read only accesses to the memory - writes will cause and access fault.

kIOMapReference will only succeed if the mapping already exists, and the IOMemoryMap object is just an extra reference, ie. no new mapping will be created.

kIOMapUnique allows a special kind of mapping to be created that may be used with the IOMemoryMap::redirect() API. These mappings will not be shared as is the default - there will always be a unique mapping created for the caller, not an existing mapping with an extra reference.

`offset`  

Is a beginning offset into the IOMemoryDescriptor's memory where the mapping starts. Zero is the default to map all the memory.

`length`  

Is the length of the mapping requested for a subset of the IOMemoryDescriptor. Zero is the default to map all the memory.

## Return Value

A reference to an IOMemoryMap object representing the mapping, which can supply the virtual address of the mapping and other information. The mapping may be shared with multiple callers - multiple maps are avoided if a compatible one exists. The IOMemoryMap object returned should be released only when the caller has finished accessing the mapping, as freeing the object destroys the mapping. The IOMemoryMap instance also retains the IOMemoryDescriptor it maps while it exists.

## Overview

This is the general purpose method to map all or part of the memory described by a memory descriptor into a task at any available address, or at a fixed address if possible. Caching & read-only options may be set for the mapping. The mapping is represented as a returned reference to a IOMemoryMap object, which may be shared if the mapping is compatible with an existing mapping of the IOMemoryDescriptor. The IOMemoryMap object returned should be released only when the caller has finished accessing the mapping, as freeing the object destroys the mapping.

## See Also

### Mapping to the Other Address Spaces

- createMappingInTask

Maps an IOMemoryDescriptor into a task.

map

Maps an IOMemoryDescriptor into the kernel map.

- map

Maps an IOMemoryDescriptor into the kernel map.

setMapping

Establishes an already existing mapping.

- setMapping

Establishes an already existing mapping.

