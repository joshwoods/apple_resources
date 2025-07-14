

- Kernel
- IOKit Fundamentals
- Memory
- IOInterleavedMemoryDescriptor
-  initWithCapacity 

# initWithCapacity

Initialize an IOInterleavedMemoryDescriptor to describe a memory area made up of several other IOMemoryDescriptors.

``` source
virtual bool initWithCapacity(
 IOByteCountcapacity, 
 IODirectiondirection ); 
```

## Parameters 

`capacity`  

The maximum number of IOMemoryDescriptors that may be subsequently added to this IOInterleavedMemoryDescriptor.

`direction`  

An I/O direction to be associated with the descriptor, which may affect the operation of the prepare and complete methods on some architectures.

## Return Value

The created IOInterleavedMemoryDescriptor on success, to be released by the caller, or zero on failure.

## Overview

This method initializes an IOInterleavedMemoryDescriptor for memory consisting of portions of a number of other IOMemoryDescriptors, chained end-to-end (in the order they appear in the array) to represent a single contiguous memory buffer.

## See Also

### Miscellaneous

clearMemoryDescriptors

Clear all of the IOMemoryDescriptors currently contained in and reset the IOInterleavedMemoryDescriptor.

complete

Complete processing of the memory after an I/O transfer finishes.

getPhysicalSegment

Break a memory descriptor into its physically contiguous segments.

prepare

Prepare the memory for an I/O transfer.

setMemoryDescriptor

Add a portion of an IOMemoryDescriptor to the IOInterleavedMemoryDescriptor.

withCapacity

Create an IOInterleavedMemoryDescriptor to describe a memory area made up of several other IOMemoryDescriptors.

