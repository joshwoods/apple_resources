

- Kernel
- IOKit Fundamentals
- Memory
-  IODMACommand 

Class

# IODMACommand

An object that converts memory references to I/O bus addresses.

DriverKitKernelDriverKit 20.0+macOS 10.4+

**DriverKit**

``` source
class IODMACommand : OSObject
```

**macOS**

``` source
class IODMACommand : IOCommand
```

## Overview

The `IODMACommand` class supersedes `IOMemoryCursor` and greatly enhances the functionality and power of it. The command can be specified to output 64 bit physical addresses and also allows driver writers to bypass mapping hardware or get addresses suitable for non-snooped DMA.

The command is designed to be very easily subclassable. Most driver writers need to associate some DMA operations with their memory descriptor, and usually use a C structure for that purpose. This structure is often kept in a linked list. This `IODMACommand` has built-in `` linkage and can be derived and 'public:' variables added, giving the developer a structure that can associate a memory descriptor with a particular DMA command but will also allow the developer to generate that command and keep the state necessary for tracking it.

Create a pool of `IODMACommand` objects at driver initialization, and keep each command in an IOCommandPool when not in use. You may also maintain your own free list of objects if preferred. See the `` and `` for sample code on manipulating the command's doubly linked list entries.

You can use an `IODMACommand` object in a 'weak-linked' manner. To do this you must avoid using any static member functions. Use the much slower, but safe, weakWithSpecification function. On success, the function returns a DMA command object, which you can use to clone as many commands as needed.

## Topics

### Creating a DMA Command

withSpecification

Creates and initializes a DMA command in one operation.

+ withSpecification

Creates and initializes an DMA command in one operation.

+ withSpecification

Creates and initializes an DMA command in one operation.

initWithSpecification

Primary initializer for the DMA command object.

- initWithSpecification

Primary initializer for the DMA command object.

- initWithSpecification

Primary initializer for the DMA command object.

weakWithSpecification

Creates and initializes an DMA command object in one operation if this version of the operating system supports it.

+ withRefCon

- initWithRefCon

cloneCommand

Creates a new command based on the specification of the current one.

- cloneCommand

Creates a new command based on the specification of the current one.

- init

- free

MappingOptions

Mapping types to indicate the desired mapper type for translating memory descriptors into I/O DMA Bus addresses.

SynchronizeOptions

Options for the synchronize method.

### Configuring the Memory Descriptor

setMemoryDescriptor

Sets and resets the DMACommand's current memory descriptor

- setMemoryDescriptor

Sets and resets the DMACommand's current memory descriptor

clearMemoryDescriptor

Clears the DMACommand's current memory descriptor

- clearMemoryDescriptor

Clears the DMACommand's current memory descriptor

getMemoryDescriptor

Get the current memory descriptor

- getMemoryDescriptor

Get the current memory descriptor

- getIOMemoryDescriptor

getPreparedOffsetAndLength

Returns the offset and length into the target IOMemoryDescriptor of a prepared IODDMACommand.

- getPreparedOffsetAndLength

Returns the offset and length into the target IOMemoryDescriptor of a prepared IODDMACommand.

genIOVMSegments

Generates a physical scatter/gather for the current DMA command

- genIOVMSegments

Generates a physical scatter/gather for the current DMA command

gen32IOVMSegments

Helper function for a type checked call to genIOVMSegments(qv), for use with an IODMACommand set up with the output function kIODMACommandOutputHost32, kIODMACommandOutputBig32, or kIODMACommandOutputLittle32. If the output function of the IODMACommand is not a 32 bit function, results will be incorrect.

- gen32IOVMSegments

gen64IOVMSegments

Helper function for a type checked call to genIOVMSegments(qv), for use with an IODMACommand set up with the output function kIODMACommandOutputHost64, kIODMACommandOutputBig64, or kIODMACommandOutputLittle64. If the output function of the IODMACommand is not a 64 bit function, results will be incorrect.

- gen64IOVMSegments

- createCopyBuffer

### Preparing the Transfer Operation

prepare

Prepare the memory for an I/O transfer.

- prepare

Prepare the memory for an I/O transfer.

prepareWithSpecification

Prepare the memory for an I/O transfer with a new specification.

- prepareWithSpecification

Prepare the memory for an I/O transfer with a new specification.

- prepareWithSpecification

Prepare the memory for an I/O transfer with a new specification.

complete

Complete processing of DMA mappings after an I/O transfer is finished.

- complete

Complete processing of DMA mappings after an I/O transfer is finished.

synchronize

Bring IOMemoryDescriptor and IODMACommand buffers into sync.

- synchronize

Bring IOMemoryDescriptor and IODMACommand buffers into sync.

### Transferring Data

readBytes

Copy data from the IODMACommand's buffer to the specified buffer.

- readBytes

Copy data from the IODMACommand's buffer to the specified buffer.

writeBytes

Copy data to the IODMACommand's buffer from the specified buffer.

- writeBytes

Copy data to the IODMACommand's buffer from the specified buffer.

### Managing Memory Segments

Segment32

A 32 bit I/O bus address/length pair.

Segment64

A 64 bit I/O bus address/length pair.

SegmentFunction

A C function that translates a 64-bit segment and outputs a single desired segment to the specified array.

kIODMACommandOutputBig32

Output big-endian Segment32 output segment function.

OutputBig32

Output big-endian Segment32 output segment function.

+ OutputBig32

Output big-endian Segment32 output segment function.

kIODMACommandOutputBig64

Output big-endian Segment64 output segment function.

OutputBig64

Output big-endian Segment64 output segment function.

+ OutputBig64

Output big-endian Segment64 output segment function.

kIODMACommandOutputHost32

Output host natural Segment32 output segment function.

OutputHost32

Output host natural Segment32 output segment function.

+ OutputHost32

Output host natural Segment32 output segment function.

kIODMACommandOutputHost64

Output host natural Segment64 output segment function.

OutputHost64

Output host natural Segment64 output segment function.

+ OutputHost64

Output host natural Segment64 output segment function.

kIODMACommandOutputLittle32

Output little-endian Segment32 output segment function.

OutputLittle32

Output little-endian Segment32 output segment function.

+ OutputLittle32

Output little-endian Segment32 output segment function.

kIODMACommandOutputLittle64

Output little-endian Segment64 output segment function.

OutputLittle64

Output little-endian Segment64 output segment function.

+ OutputLittle64

Output little-endian Segment64 output segment function.

### Getting Configuration Details

- getAlignment

- getAlignmentInternalSegments

- getAlignmentLength

- getMetaClass

- getNumAddressBits

- setSpecification

### Performing Internal Operations

Private Accessors

### Type Methods

+ weakWithSpecification

## Relationships

### Inherits From

- IOCommand
- OSObject

## See Also

### Direct Memory Access (DMA)

IODMAController

IODMAEventSource

