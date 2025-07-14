

- Kernel
- IOKit Fundamentals
- Memory
-  IOInterleavedMemoryDescriptor 

Class

# IOInterleavedMemoryDescriptor

The IOInterleavedMemoryDescriptor object describes a memory area made up of portions of several other IOMemoryDescriptors.

macOS 10.5+

``` source
class IOInterleavedMemoryDescriptor : IOMemoryDescriptor
```

## Overview

The IOInterleavedMemoryDescriptor object represents interleaved ranges of memory, specified as an ordered list of portions of individual IOMemoryDescriptors. The portions are chained end-to-end to make up a single contiguous buffer.

## Topics

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

setMemoryDescriptor

Add a portion of an IOMemoryDescriptor to the IOInterleavedMemoryDescriptor.

withCapacity

Create an IOInterleavedMemoryDescriptor to describe a memory area made up of several other IOMemoryDescriptors.

### Instance Methods

- clearMemoryDescriptors

- complete

- free

- getMetaClass

- getPhysicalSegment

- initWithCapacity

- prepare

- setMemoryDescriptor

### Type Methods

+ withCapacity

## Relationships

### Inherits From

- IOMemoryDescriptor

## See Also

### Descriptors

IOBufferMemoryDescriptor

A simple memory descriptor that allocates its own buffer memory.

IODeviceMemory

An IOMemoryDescriptor used for device physical memory ranges.

IOGeneralMemoryDescriptor

IOMultiMemoryDescriptor

The IOMultiMemoryDescriptor object describes a memory area made up of several other IOMemoryDescriptors.

IOSubMemoryDescriptor

The IOSubMemoryDescriptor object describes a memory area made up of a portion of another IOMemoryDescriptor.

IOMemoryDescriptor

An abstract base class that defines common methods for describing physical or virtual memory.

