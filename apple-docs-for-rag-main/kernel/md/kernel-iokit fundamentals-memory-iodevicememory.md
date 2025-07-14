

- Kernel
- IOKit Fundamentals
- Memory
-  IODeviceMemory 

Class

# IODeviceMemory

An IOMemoryDescriptor used for device physical memory ranges.

macOS 10.0+

``` source
class IODeviceMemory : IOMemoryDescriptor
```

## Overview

The IODeviceMemory class is a simple subclass of IOMemoryDescriptor that uses its methods to describe a single range of physical memory on a device. IODeviceMemory objects are usually looked up with IOService or IOPCIDevice accessors, and are created by memory-mapped bus families. IODeviceMemory implements only some factory methods in addition to the methods of IOMemoryDescriptor.

## Topics

### Miscellaneous

arrayFromList

Constructs an OSArray of IODeviceMemory instances, each describing one physical range, and a tag value.

withRange

Constructs an IODeviceMemory instance, describing one physical range.

withSubRange

Constructs an IODeviceMemory instance, describing a subset of an existing IODeviceMemory range.

### DataTypes

InitElement

### Instance Methods

- getMetaClass

### Type Methods

+ arrayFromList

+ withRange

+ withSubRange

## Relationships

### Inherits From

- IOMemoryDescriptor

## See Also

### Descriptors

IOBufferMemoryDescriptor

A simple memory descriptor that allocates its own buffer memory.

IOGeneralMemoryDescriptor

IOInterleavedMemoryDescriptor

The IOInterleavedMemoryDescriptor object describes a memory area made up of portions of several other IOMemoryDescriptors.

IOMultiMemoryDescriptor

The IOMultiMemoryDescriptor object describes a memory area made up of several other IOMemoryDescriptors.

IOSubMemoryDescriptor

The IOSubMemoryDescriptor object describes a memory area made up of a portion of another IOMemoryDescriptor.

IOMemoryDescriptor

An abstract base class that defines common methods for describing physical or virtual memory.

