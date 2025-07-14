

- DriverKit
-  IOMemoryDescriptor 

Class

# IOMemoryDescriptor

The base class for describing a location in memory.

DriverKitiOSiPadOSmacOS

``` source
class IOMemoryDescriptor;
```

## Overview

The IOMemoryDescriptor class defines shared behavior for memory-related objects. Use the methods of this class to get information about a memory block and to map a memory block from another process into your driver’s memory space.

Don’t create instances of this class directly. When you want to allocate memory for your driver, create an IOBufferMemoryDescriptor instead, which is a concrete implementation of this class.

## Topics

### Configuring the Buffer

init

Initializes the memory descriptor object.

free

Performs any final cleanup for the memory descriptor object.

### Getting the Buffer Length

GetLength

Returns the length of the memory block represented by this object.

### Mapping to the Caller’s Address Space

CreateMapping

Maps the contents of the memory block to the address space of the current process.

Memory Map Options

Options that describe how to configure a memory-mapped buffer.

### Performing Internal Tasks

Map

Maps memory internally.

### Type Methods

CreateSubMemoryDescriptor

CreateWithMemoryDescriptors

## Relationships

### Inherits From

- OSObject

### Inherited By

- IOBufferMemoryDescriptor

## See Also

### Memory management

IOBufferMemoryDescriptor

A memory buffer allocated in the caller’s address space.

IOMemoryMap

A reference to an existing block of memory in the current process or in a different process.

Memory Utilities

Allocate and deallocate memory and manage memory pointers in different address spaces.

