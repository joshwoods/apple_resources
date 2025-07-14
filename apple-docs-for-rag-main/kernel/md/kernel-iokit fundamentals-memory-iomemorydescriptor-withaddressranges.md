

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryDescriptor
-  withAddressRanges 

# withAddressRanges

Creates an IOMemoryDescriptor to describe one or more virtual ranges.

``` source
static IOMemoryDescriptor * withAddressRanges( 
 IOAddressRange *ranges, 
 UInt32rangeCount, 
 IOOptionBitsoptions, 
 task_ttask); 
```

## Parameters 

`ranges`  

An array of IOAddressRange structures which specify the virtual ranges in the specified map which make up the memory to be described. IOAddressRange is the 64bit version of IOVirtualRange.

`rangeCount`  

The member count of the ranges array.

`options`  

kIOMemoryDirectionMask (options:direction) This nibble indicates the I/O direction to be associated with the descriptor, which may affect the operation of the prepare and complete methods on some architectures. kIOMemoryAsReference For options:type = Virtual or Physical this indicate that the memory descriptor need not copy the ranges array into local memory. This is an optimisation to try to minimise unnecessary allocations.

`task`  

The task each of the virtual ranges are mapped into. Note that unlike IOMemoryDescriptor::withAddress(), kernel_task memory must be explicitly prepared when passed to this api. The task argument may be NULL to specify memory by physical address.

## Return Value

The created IOMemoryDescriptor on success, to be released by the caller, or zero on failure.

## Overview

This method creates and initializes an IOMemoryDescriptor for memory consisting of an array of virtual memory ranges each mapped into a specified source task. This memory descriptor needs to be prepared before it can be used to extract data from the memory described.

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

