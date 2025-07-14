

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryDescriptor
-  initWithOptions 

# initWithOptions

Primary initializer for all variants of memory descriptors.

``` source
virtual bool initWithOptions(
 void *buffers, 
 UInt32 count, 
 UInt32 offset, 
 task_t task, 
 IOOptionBits options, 
 IOMapper *mapper = kIOMapperSystem); 
```

## Return Value

true on success, false on failure.

## Overview

Note this function can be used to re-init a previously created memory descriptor. For a more complete description see withOptions.

## See Also

### Creating the Memory Buffer

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

withPhysicalAddress

Creates an IOMemoryDescriptor to describe one physical range.

+ withPhysicalAddress

Creates an IOMemoryDescriptor to describe one physical range.

- free

Performs any final cleanup for the memory descriptor object.

