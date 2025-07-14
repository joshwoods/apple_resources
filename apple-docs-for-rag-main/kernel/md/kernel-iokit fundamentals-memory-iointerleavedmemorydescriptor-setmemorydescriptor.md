

- Kernel
- IOKit Fundamentals
- Memory
- IOInterleavedMemoryDescriptor
-  setMemoryDescriptor 

# setMemoryDescriptor

Add a portion of an IOMemoryDescriptor to the IOInterleavedMemoryDescriptor.

``` source
virtual bool setMemoryDescriptor(
 IOMemoryDescriptor *descriptor, 
 IOByteCountoffset, 
 IOByteCountlength ); 
```

## Parameters 

`descriptor`  

An IOMemoryDescriptor to be added to the IOInterleavedMemoryDescriptor. Its direction must be compatible with that of the IOInterleavedMemoryDescriptor.

`offset`  

The offset into the IOMemoryDescriptor of the portion that will be added to the virtualized buffer.

`length`  

The length of the portion of the IOMemoryDescriptor to be added to the virtualized buffer.

## Return Value

Returns true the portion was successfully added.

## Overview

This method adds the portion of an IOMemoryDescriptor described by the offset and length parameters to the end of the IOInterleavedMemoryDescriptor. A single IOMemoryDescriptor may be added as many times as there is room for it. The offset and length must describe a portion entirely within the IOMemoryDescriptor.

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

prepare

Prepare the memory for an I/O transfer.

withCapacity

Create an IOInterleavedMemoryDescriptor to describe a memory area made up of several other IOMemoryDescriptors.

