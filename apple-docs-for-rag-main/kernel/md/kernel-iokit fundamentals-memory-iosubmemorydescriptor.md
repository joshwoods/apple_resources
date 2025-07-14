

- Kernel
- IOKit Fundamentals
- Memory
-  IOSubMemoryDescriptor 

Class

# IOSubMemoryDescriptor

The IOSubMemoryDescriptor object describes a memory area made up of a portion of another IOMemoryDescriptor.

macOS 10.0+

``` source
class IOSubMemoryDescriptor : IOMemoryDescriptor
```

## Overview

The IOSubMemoryDescriptor object represents a subrange of memory, specified as a portion of another IOMemoryDescriptor.

## Topics

### Miscellaneous

withSubRange

Create an IOMemoryDescriptor to describe a subrange of an existing descriptor.

### Instance Methods

- complete

- free

- getMetaClass

- getPageCounts

- getPhysicalSegment

- getPreparationID

- initSubRange

- makeMapping

- prepare

- redirect

- setOwnership

- setPurgeable

### Type Methods

+ withSubRange

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

IOMultiMemoryDescriptor

The IOMultiMemoryDescriptor object describes a memory area made up of several other IOMemoryDescriptors.

IOMemoryDescriptor

An abstract base class that defines common methods for describing physical or virtual memory.

