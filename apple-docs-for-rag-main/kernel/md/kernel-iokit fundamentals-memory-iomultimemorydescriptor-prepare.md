

- Kernel
- IOKit Fundamentals
- Memory
- IOMultiMemoryDescriptor
-  prepare 

# prepare

Prepare the memory for an I/O transfer.

``` source
virtual IOReturn prepare(
 IODirection forDirection = forDirection); 
```

## Parameters 

`forDirection`  

The direction of the I/O just completed, or kIODirectionNone for the direction specified by the memory descriptor.

## Return Value

An IOReturn code.

## Overview

This involves paging in the memory, if necessary, and wiring it down for the duration of the transfer. The complete() method completes the processing of the memory after the I/O transfer finishes. This method needn't called for non-pageable memory.

## See Also

### Miscellaneous

complete

Complete processing of the memory after an I/O transfer finishes.

getPhysicalSegment

Break a memory descriptor into its physically contiguous segments.

initWithDescriptors

Initialize an IOMultiMemoryDescriptor to describe a memory area made up of several other IOMemoryDescriptors.

withDescriptors(IOMemoryDescriptor **, UInt32, IODirection, bool)

Create an IOMultiMemoryDescriptor to describe a memory area made up of several other IOMemoryDescriptors.

withDescriptors(IOMemoryDescriptor **, UInt32, IODirection, bool)

Initialize an IOMultiMemoryDescriptor to describe a memory area made up of several other IOMemoryDescriptors.

