

- Kernel
- IOKit Fundamentals
- Memory
- IOInterleavedMemoryDescriptor
-  clearMemoryDescriptors 

# clearMemoryDescriptors

Clear all of the IOMemoryDescriptors currently contained in and reset the IOInterleavedMemoryDescriptor.

``` source
virtual void clearMemoryDescriptors(
 IODirection direction = direction ); 
```

## Parameters 

`direction`  

An I/O direction to be associated with the descriptor, which may affect the operation of the prepare and complete methods on some architectures.

## Overview

Clears each IOMemoryDescriptor by completing (if needed) and releasing. The IOInterleavedMemoryDescriptor is then reset and may accept new descriptors up to the capacity specified when it was created.

## See Also

### Miscellaneous

complete

Complete processing of the memory after an I/O transfer finishes.

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

