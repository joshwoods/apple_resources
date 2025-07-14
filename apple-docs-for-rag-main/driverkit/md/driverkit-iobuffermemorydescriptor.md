

- DriverKit
-  IOBufferMemoryDescriptor 

Class

# IOBufferMemoryDescriptor

A memory buffer allocated in the caller’s address space.

DriverKitiOSiPadOSmacOS

``` source
class IOBufferMemoryDescriptor;
```

## Overview

Use an IOBufferMemoryDescriptor to share data between your driver and other processes, including the kernel. You create memory buffers in your driver’s process space, but you can pass the buffer to any API that expects an IOMemoryDescriptor object. Some DriverKit APIs pass your buffer to another process, which can then map the buffer to its own address space and access the contents.

Typically, you create memory buffer objects to store data moving in and out of your driver. For example, a network interface driver might create a buffer to store packet data it receives from the associated device. You are responsible for managing the contents of the buffer yourself, typically by mapping it to a known data type. Except where noted, you are also responsible for releasing buffers that you allocate.

## Topics

### Creating a Memory Buffer

Create

Creates a new memory buffer descriptor object in the current process space.

init

Initializes the buffer memory descriptor object.

free

Performs any final cleanup for the memory buffer descriptor object.

### Managing the Buffer Contents

SetLength

Changes the length of the memory buffer.

GetAddressRange

Returns the address and length of the memory buffer.

IOAddressSegment

A structure that describes the location and size of a block of memory.

## Relationships

### Inherits From

- IOMemoryDescriptor

## See Also

### Memory management

IOMemoryDescriptor

The base class for describing a location in memory.

IOMemoryMap

A reference to an existing block of memory in the current process or in a different process.

Memory Utilities

Allocate and deallocate memory and manage memory pointers in different address spaces.

