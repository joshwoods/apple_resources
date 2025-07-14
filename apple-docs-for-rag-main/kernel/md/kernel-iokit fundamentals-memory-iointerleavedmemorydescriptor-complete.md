

- Kernel
- IOKit Fundamentals
- Memory
- IOInterleavedMemoryDescriptor
-  complete 

# complete

Complete processing of the memory after an I/O transfer finishes.

``` source
virtual IOReturn complete(
 IODirection forDirection = forDirection); 
```

## Parameters 

`forDirection`  

The direction of the I/O just completed, or kIODirectionNone for the direction specified by the memory descriptor.

## Return Value

An IOReturn code.

## Overview

This method should not be called unless a prepare was previously issued; the prepare() and complete() must occur in pairs, before and after an I/O transfer involving pageable memory.

## See Also

### Miscellaneous

clearMemoryDescriptors

Clear all of the IOMemoryDescriptors currently contained in and reset the IOInterleavedMemoryDescriptor.

getPhysicalSegment

Break a memory descriptor into its physically contiguous segments.

initWithCapacity

Initialize an IOInterleavedMemoryDescriptor to describe a memory area made up of several other IOMemoryDescriptors.

prepare

Prepare the memory for an I/O transfer.

setMemoryDescriptor

Add a portion of an IOMemoryDescriptor to the IOInterleavedMemoryDescriptor.

withCapacity

Create an IOInterleavedMemoryDescriptor to describe a memory area made up of several other IOMemoryDescriptors.

