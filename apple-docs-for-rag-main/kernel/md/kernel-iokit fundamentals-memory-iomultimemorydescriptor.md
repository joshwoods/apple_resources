

- Kernel
- IOKit Fundamentals
- Memory
-  IOMultiMemoryDescriptor 

Class

# IOMultiMemoryDescriptor

The IOMultiMemoryDescriptor object describes a memory area made up of several other IOMemoryDescriptors.

macOS 10.0+

``` source
class IOMultiMemoryDescriptor : IOMemoryDescriptor
```

## Overview

The IOMultiMemoryDescriptor object represents multiple ranges of memory, specified as an ordered list of IOMemoryDescriptors. The descriptors are chained end-to-end to make up a single contiguous buffer.

## Topics

### Miscellaneous

complete

Complete processing of the memory after an I/O transfer finishes.

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

### Instance Methods

- complete

- doMap

- free

- getMetaClass

- getPageCounts

- getPhysicalSegment

- getPreparationID

- initWithDescriptors

- prepare

- setOwnership

- setPurgeable

### Type Methods

+ withDescriptors

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

IOInterleavedMemoryDescriptor

The IOInterleavedMemoryDescriptor object describes a memory area made up of portions of several other IOMemoryDescriptors.

IOSubMemoryDescriptor

The IOSubMemoryDescriptor object describes a memory area made up of a portion of another IOMemoryDescriptor.

IOMemoryDescriptor

An abstract base class that defines common methods for describing physical or virtual memory.

