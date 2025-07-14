

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryDescriptor
-  map 

# map

Maps an IOMemoryDescriptor into the kernel map.

``` source
virtual IOMemoryMap * map( 
 IOOptionBits options = 0 ); 
```

## Parameters 

`options`  

Mapping options as in the full version of the createMappingInTask method, with kIOMapAnywhere assumed.

## Return Value

See the full version of the createMappingInTask method.

## Overview

This is a shortcut method to map all the memory described by a memory descriptor into the kernel map at any available address. See the full version of the createMappingInTask method for further details.

## See Also

### Mapping to the Other Address Spaces

createMappingInTask

Maps an IOMemoryDescriptor into a task.

- createMappingInTask

Maps an IOMemoryDescriptor into a task.

- map

Maps an IOMemoryDescriptor into the kernel map.

setMapping

Establishes an already existing mapping.

- setMapping

Establishes an already existing mapping.

