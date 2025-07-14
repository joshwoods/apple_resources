

- Kernel
- IOKit Fundamentals
- Memory
-  IOBufferMemoryDescriptor 

Class

# IOBufferMemoryDescriptor

A simple memory descriptor that allocates its own buffer memory.

macOS 10.0+

``` source
class IOBufferMemoryDescriptor : IOGeneralMemoryDescriptor
```

## Overview

Use an `IOBufferMemoryDescriptor` object to store data and share it with the kernel.

## Topics

### Creating a Memory Buffer Descriptor

inTaskWithOptions

Creates a memory buffer with memory descriptor for that buffer.

+ inTaskWithOptions

Creates a memory buffer with memory descriptor for that buffer.

+ inTaskWithOptions

Creates a memory buffer with memory descriptor for that buffer.

inTaskWithPhysicalMask

Creates a memory buffer with memory descriptor for that buffer.

+ inTaskWithPhysicalMask

Creates a memory buffer with memory descriptor for that buffer.

- initWithPhysicalMask

Creates a memory buffer with memory descriptor for that buffer.

+ withOptions

Creates a memory buffer with memory descriptor for that buffer.

+ withBytes

Creates a buffer memory descriptor and fills it with the specified bytes.

+ withCapacity

Creates a buffer memory descriptor and allocates enough bytes to meet the specified capacity.

+ withCopy

Creates a memory buffer with memory descriptor for that buffer.

- free

Performs any final cleanup for the memory buffer descriptor object.

### Configuring the Descriptor

- getCapacity

Returns the number of bytes the buffer is capable of holding.

- setDirection

Changes the direction associated with the buffer’s memory transfers.

- setLength

Sets the length of the data in the buffer.

### Adding Data to the Buffer

- appendBytes

Adds the specified data to the end of the memory buffer.

### Getting the Buffer Contents

- getBytesNoCopy

Returns the virtual address of the beginning of the memory buffer.

- getBytesNoCopy

Returns the virtual address of an offset into the memory buffer.

### Managing Internal Structures

ExpansionData

reserved

+ Create

Creates a new memory buffer descriptor object in the current process space.

+ Create_Impl

+ Create_Invoke

- GetAddressRange

Returns the address and length of the memory buffer.

- getMetaClass

+ SetLength_Invoke

- SetLength

Changes the length of the memory buffer.

- SetLength_Impl

- Dispatch

## Relationships

### Inherits From

- IOGeneralMemoryDescriptor

## See Also

### Descriptors

IODeviceMemory

An IOMemoryDescriptor used for device physical memory ranges.

IOGeneralMemoryDescriptor

IOInterleavedMemoryDescriptor

The IOInterleavedMemoryDescriptor object describes a memory area made up of portions of several other IOMemoryDescriptors.

IOMultiMemoryDescriptor

The IOMultiMemoryDescriptor object describes a memory area made up of several other IOMemoryDescriptors.

IOSubMemoryDescriptor

The IOSubMemoryDescriptor object describes a memory area made up of a portion of another IOMemoryDescriptor.

IOMemoryDescriptor

An abstract base class that defines common methods for describing physical or virtual memory.

