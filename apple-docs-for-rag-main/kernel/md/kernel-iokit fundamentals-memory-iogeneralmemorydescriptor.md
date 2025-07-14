

- Kernel
- IOKit Fundamentals
- Memory
-  IOGeneralMemoryDescriptor 

Class

# IOGeneralMemoryDescriptor

macOS 10.0+

``` source
class IOGeneralMemoryDescriptor : IOMemoryDescriptor
```

## Topics

### Instance Methods

- complete

- dmaCommandOperation

- doMap

- doUnmap

- free

- getMetaClass

- getPhysicalSegment

- getPreparationID

- initWithOptions

- makeMapping

- makeMapping

- memoryReferenceCreateOptions

- prepare

- serialize

- setOwnership

- setPurgeable

### Type Methods

+ withPersistentMemoryDescriptor

## Relationships

### Inherits From

- IOMemoryDescriptor

## See Also

### Descriptors

IOBufferMemoryDescriptor

A simple memory descriptor that allocates its own buffer memory.

IODeviceMemory

An IOMemoryDescriptor used for device physical memory ranges.

IOInterleavedMemoryDescriptor

The IOInterleavedMemoryDescriptor object describes a memory area made up of portions of several other IOMemoryDescriptors.

IOMultiMemoryDescriptor

The IOMultiMemoryDescriptor object describes a memory area made up of several other IOMemoryDescriptors.

IOSubMemoryDescriptor

The IOSubMemoryDescriptor object describes a memory area made up of a portion of another IOMemoryDescriptor.

IOMemoryDescriptor

An abstract base class that defines common methods for describing physical or virtual memory.

