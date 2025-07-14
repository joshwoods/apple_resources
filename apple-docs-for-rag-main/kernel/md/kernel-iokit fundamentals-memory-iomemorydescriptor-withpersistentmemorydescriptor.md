

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryDescriptor
-  withPersistentMemoryDescriptor 

# withPersistentMemoryDescriptor

Copy constructor that generates a new memory descriptor if the backing memory for the same task's virtual address and length has changed.

``` source
static IOMemoryDescriptor * withPersistentMemoryDescriptor(
 IOMemoryDescriptor *originalMD); 
```

## Parameters 

`originalMD`  

The memory descriptor to be duplicated.

## Return Value

Either the original memory descriptor with an additional retain or a new memory descriptor, 0 for a bad original memory descriptor or some other resource shortage.

## Overview

If the original memory descriptor's address and length is still backed by the same real memory, i.e. the user hasn't deallocated and the reallocated memory at the same address then the original memory descriptor is returned with a additional reference. Otherwise we build a totally new memory descriptor with the same characteristics as the previous one but with a new view of the vm. Note not legal to call this function with anything except an IOGeneralMemoryDescriptor that was created with the kIOMemoryPersistent option.

## See Also

### Creating the Memory Buffer

initWithOptions

Primary initializer for all variants of memory descriptors.

- initWithOptions

Primary initializer for all variants of memory descriptors.

withOptions

Primary initializer for all variants of memory descriptors.

+ withOptions

Primary initializer for all variants of memory descriptors.

withAddress

Creates an IOMemoryDescriptor to describe one virtual range of the kernel task.

+ withAddress

Creates an IOMemoryDescriptor to describe one virtual range of the kernel task.

withAddressRange

Creates an IOMemoryDescriptor to describe one virtual range of the specified map.

+ withAddressRange

Creates an IOMemoryDescriptor to describe one virtual range of the specified map.

withAddressRanges

Creates an IOMemoryDescriptor to describe one or more virtual ranges.

+ withAddressRanges

Creates an IOMemoryDescriptor to describe one or more virtual ranges.

+ withPersistentMemoryDescriptor

Copy constructor that generates a new memory descriptor if the backing memory for the same task's virtual address and length has changed.

withPhysicalAddress

Creates an IOMemoryDescriptor to describe one physical range.

+ withPhysicalAddress

Creates an IOMemoryDescriptor to describe one physical range.

- free

Performs any final cleanup for the memory descriptor object.

