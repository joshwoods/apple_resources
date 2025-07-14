

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryDescriptor
-  setMapping 

# setMapping

Establishes an already existing mapping.

``` source
virtual IOMemoryMap * setMapping( 
 task_t task, 
 IOVirtualAddress mapAddress, 
 IOOptionBits options = 0 ); 
```

## Parameters 

`task`  

Address space in which the mapping exists.

`mapAddress`  

Virtual address of the mapping.

`options`  

Caching and read-only attributes of the mapping.

## Return Value

A IOMemoryMap object created to represent the mapping.

## Overview

This method tells the IOMemoryDescriptor about a mapping that exists, but was created elsewhere. It allows later callers of the map method to share this externally created mapping. The IOMemoryMap object returned is created to represent it. This method is not commonly needed.

## See Also

### Mapping to the Other Address Spaces

createMappingInTask

Maps an IOMemoryDescriptor into a task.

- createMappingInTask

Maps an IOMemoryDescriptor into a task.

map

Maps an IOMemoryDescriptor into the kernel map.

- map

Maps an IOMemoryDescriptor into the kernel map.

- setMapping

Establishes an already existing mapping.

