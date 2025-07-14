

- Kernel
- IOKit Fundamentals
- Memory
- IOMultiMemoryDescriptor
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

getPhysicalSegment

Break a memory descriptor into its physically contiguous segments.

initWithDescriptors

Initialize an IOMultiMemoryDescriptor to describe a memory area made up of several other IOMemoryDescriptors.

prepare

Prepare the memory for an I/O transfer.

withDescriptors(IOMemoryDescriptor **, UInt32, IODirection, bool)

Create an IOMultiMemoryDescriptor to describe a memory area made up of several other IOMemoryDescriptors.

withDescriptors(IOMemoryDescriptor **, UInt32, IODirection, bool)

Initialize an IOMultiMemoryDescriptor to describe a memory area made up of several other IOMemoryDescriptors.

