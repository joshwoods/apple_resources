

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryDescriptor
-  withPhysicalAddress 

# withPhysicalAddress

Creates an IOMemoryDescriptor to describe one physical range.

``` source
static IOMemoryDescriptor * withPhysicalAddress( 
 IOPhysicalAddressaddress, 
 IOByteCountwithLength, 
 IODirectionwithDirection ); 
```

## Parameters 

`address`  

The physical address of the first byte in the memory.

`withLength`  

The length of memory.

`withDirection`  

An I/O direction to be associated with the descriptor, which may affect the operation of the prepare and complete methods on some architectures.

## Return Value

The created IOMemoryDescriptor on success, to be released by the caller, or zero on failure.

## Overview

This method creates and initializes an IOMemoryDescriptor for memory consisting of a single physical memory range.

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

withPersistentMemoryDescriptor

Copy constructor that generates a new memory descriptor if the backing memory for the same task's virtual address and length has changed.

+ withPersistentMemoryDescriptor

Copy constructor that generates a new memory descriptor if the backing memory for the same task's virtual address and length has changed.

+ withPhysicalAddress

Creates an IOMemoryDescriptor to describe one physical range.

- free

Performs any final cleanup for the memory descriptor object.

