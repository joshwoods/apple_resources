

- Kernel
- IOKit Fundamentals
- Memory
-  IOMemoryDescriptor 

Class

# IOMemoryDescriptor

An abstract base class that defines common methods for describing physical or virtual memory.

macOS 10.0+

``` source
class IOMemoryDescriptor : OSObject
```

## Overview

An `IOMemoryDescriptor` object represents a buffer or range of memory, specified as one or more physical or virtual address ranges. It contains methods to return the memory's physically contiguous segments (fragments), for use with the IOMemoryCursor, and methods to map the memory into any address space with caching and placed mapping options.

## Topics

### Creating the Memory Buffer

initWithOptions

Primary initializer for all variants of memory descriptors.

- initWithOptions

Primary initializer for all variants of memory descriptors.

withOptions

Primary initializer for all variants of memory descriptors.

+ withOptions

Primary initializer for all variants of memory descriptors.

withAddress

Creates an IOMemoryDescriptor to describe one virtual range of the kernel task.

+ withAddress

Creates an IOMemoryDescriptor to describe one virtual range of the kernel task.

withAddressRange

Creates an IOMemoryDescriptor to describe one virtual range of the specified map.

+ withAddressRange

Creates an IOMemoryDescriptor to describe one virtual range of the specified map.

withAddressRanges

Creates an IOMemoryDescriptor to describe one or more virtual ranges.

+ withAddressRanges

Creates an IOMemoryDescriptor to describe one or more virtual ranges.

withPersistentMemoryDescriptor

Copy constructor that generates a new memory descriptor if the backing memory for the same task's virtual address and length has changed.

+ withPersistentMemoryDescriptor

Copy constructor that generates a new memory descriptor if the backing memory for the same task's virtual address and length has changed.

withPhysicalAddress

Creates an IOMemoryDescriptor to describe one physical range.

+ withPhysicalAddress

Creates an IOMemoryDescriptor to describe one physical range.

- free

Performs any final cleanup for the memory descriptor object.

### Configuring the Descriptor

- setOwnership

Set the task that owns the descriptor’s memory.

setPurgeable

Control the purgeable status of a memory descriptors memory.

- setPurgeable

Control the purgeable status of a memory descriptors memory.

### Preparing the Buffer

prepare

Prepare the memory for an I/O transfer.

- prepare

Prepare the memory for an I/O transfer.

complete

Complete processing of the memory after an I/O transfer finishes.

- complete

Complete processing of the memory after an I/O transfer finishes.

- getPreparationID

- setPreparationID

### Reading and Writing Buffer Data

readBytes

Copy data from the memory descriptor's buffer to the specified buffer.

- readBytes

Copy data from the memory descriptor's buffer to the specified buffer.

writeBytes

Copy data to the memory descriptor's buffer from the specified buffer.

- writeBytes

Copy data to the memory descriptor's buffer from the specified buffer.

### Mapping to the Other Address Spaces

createMappingInTask

Maps an IOMemoryDescriptor into a task.

- createMappingInTask

Maps an IOMemoryDescriptor into a task.

map

Maps an IOMemoryDescriptor into the kernel map.

- map

Maps an IOMemoryDescriptor into the kernel map.

setMapping

Establishes an already existing mapping.

- setMapping

Establishes an already existing mapping.

### Getting the Memory Pages

getPageCounts

Retrieve the number of resident and/or dirty pages encompassed by a memory descriptor.

- getPageCounts

Retrieve the number of resident and/or dirty pages encompassed by a memory descriptor.

getPhysicalAddress

Return the physical address of the first byte in the memory.

- getPhysicalAddress

Return the physical address of the first byte in the memory.

getPhysicalSegment

Break a memory descriptor into its physically contiguous segments.

- getPhysicalSegment

Break a memory descriptor into its physically contiguous segments.

### Getting the Descriptor Information

getDirection

Gets the direction of memory transfers associated with the descriptor.

- getDirection

Gets the direction of memory transfers associated with the descriptor.

getLength

Accessor to get the length of the memory descriptor (over all its ranges).

- getLength

Accessor to get the length of the memory descriptor (over all its ranges).

- GetLength

Returns the length of the memory block represented by this object.

- getDMAMapLength

- getFlags

Returns the options used to create the memory descriptor.

- getMetaClass

### Accessing the Buffer's Tag

getTag

Accessor to the retrieve the tag for the memory descriptor.

- getTag

Accessor to the retrieve the tag for the memory descriptor.

setTag

Set the tag for the memory descriptor.

- setTag

Set the tag for the memory descriptor.

- getVMTag

- setVMTags

### Operating on the Memory

performOperation

Perform an operation on the memory descriptor's memory.

- performOperation

Perform an operation on the memory descriptor's memory.

- dmaCommandOperation

### Managing Internal Structures

reserved

+ initialize

- Dispatch

+ CreateMapping_Invoke

- populateDevicePager

- CreateMapping

- CreateMapping_Impl

- Map

Maps memory internally.

- addMapping

- removeMapping

- makeMapping

- doMap

- doUnmap

- handleFault

- redirect

### Instance Methods

- getMapperOptions

- setMapperOptions

### Type Methods

+ CreateSubMemoryDescriptor

+ CreateSubMemoryDescriptor_Impl

+ CreateSubMemoryDescriptor_Invoke

+ CreateWithMemoryDescriptors

+ CreateWithMemoryDescriptors_Impl

+ CreateWithMemoryDescriptors_Invoke

## Relationships

### Inherits From

- OSObject

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

IOSubMemoryDescriptor

The IOSubMemoryDescriptor object describes a memory area made up of a portion of another IOMemoryDescriptor.

