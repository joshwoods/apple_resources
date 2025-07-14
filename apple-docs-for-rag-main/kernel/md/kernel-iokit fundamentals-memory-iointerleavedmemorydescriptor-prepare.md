

- Kernel
- IOKit Fundamentals
- Memory
- IOInterleavedMemoryDescriptor
-  prepare 

# prepare

Prepare the memory for an I/O transfer.

``` source
virtual IOReturn prepare(
 IODirection forDirection = forDirection); 
```

## Parameters 

`forDirection`  

The direction of the I/O to be performed, or kIODirectionNone for the direction specified by the memory descriptor.

## Return Value

An IOReturn code.

## Overview

This involves paging in the memory, if necessary, and wiring it down for the duration of the transfer. The complete() method completes the processing of the memory after the I/O transfer finishes. This method need not called for non-pageable memory.

## See Also

### Miscellaneous

clearMemoryDescriptors

Clear all of the IOMemoryDescriptors currently contained in and reset the IOInterleavedMemoryDescriptor.

complete

Complete processing of the memory after an I/O transfer finishes.

getPhysicalSegment

Break a memory descriptor into its physically contiguous segments.

initWithCapacity

Initialize an IOInterleavedMemoryDescriptor to describe a memory area made up of several other IOMemoryDescriptors.

setMemoryDescriptor

Add a portion of an IOMemoryDescriptor to the IOInterleavedMemoryDescriptor.

withCapacity

Create an IOInterleavedMemoryDescriptor to describe a memory area made up of several other IOMemoryDescriptors.

