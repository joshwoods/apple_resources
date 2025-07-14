

- Core Media
-  CMBlockBuffer APIs 

API Collection

# CMBlockBuffer APIs

An object the system uses to move blocks of memory through a processing system.

## Overview

A block buffer is a `CFType` object that represents a contiguous range of data offsets (from zero to CMBlockBufferGetDataLength(_:)) across a possibly noncontiguous memory region. The memory region contains memory blocks and buffer references. The buffer references can in turn refer to additional regions. `CMBlockBuffer` uses CMAttachmentBearerProtocol to propagate attachments.

## Topics

### Creating a Block Buffer

func CMBlockBufferCreateEmpty(allocator: CFAllocator?, capacity: UInt32, flags: CMBlockBufferFlags, blockBufferOut: UnsafeMutablePointer&lt;CMBlockBuffer?>) -> OSStatus

Creates an empty block buffer.

func CMBlockBufferCreateWithMemoryBlock(allocator: CFAllocator?, memoryBlock: UnsafeMutableRawPointer?, blockLength: Int, blockAllocator: CFAllocator?, customBlockSource: UnsafePointer&lt;CMBlockBufferCustomBlockSource>?, offsetToData: Int, dataLength: Int, flags: CMBlockBufferFlags, blockBufferOut: UnsafeMutablePointer&lt;CMBlockBuffer?>) -> OSStatus

Creates a block buffer that’s backed by a memory block.

func CMBlockBufferCreateWithBufferReference(allocator: CFAllocator?, referenceBuffer: CMBlockBuffer, offsetToData: Int, dataLength: Int, flags: CMBlockBufferFlags, blockBufferOut: UnsafeMutablePointer&lt;CMBlockBuffer?>) -> OSStatus

Creates a block buffer that refers to another block buffer object.

func CMBlockBufferCreateContiguous(allocator: CFAllocator?, sourceBuffer: CMBlockBuffer, blockAllocator: CFAllocator?, customBlockSource: UnsafePointer&lt;CMBlockBufferCustomBlockSource>?, offsetToData: Int, dataLength: Int, flags: CMBlockBufferFlags, blockBufferOut: UnsafeMutablePointer&lt;CMBlockBuffer?>) -> OSStatus

Creates a block buffer that contains a contiguous copy of, or reference to, the data specified by the parameters.

typealias CMBlockBufferFlags

A type for flags that control behaviors and features of block buffer APIs.

Block Buffer Flags

An enumeration of flags that control behaviors and features of block buffer APIs.

struct CMBlockBufferCustomBlockSource

A structure to support custom memory allocation and deallocation for a block used in a block buffer.

Custom Block Source Version

A custom block source version identifier.

### Modifying a Block Buffer

func CMBlockBufferAppendMemoryBlock(CMBlockBuffer, memoryBlock: UnsafeMutableRawPointer?, length: Int, blockAllocator: CFAllocator?, customBlockSource: UnsafePointer&lt;CMBlockBufferCustomBlockSource>?, offsetToData: Int, dataLength: Int, flags: CMBlockBufferFlags) -> OSStatus

Adds a memory block to an existing block buffer.

func CMBlockBufferAppendBufferReference(CMBlockBuffer, targetBBuf: CMBlockBuffer, offsetToData: Int, dataLength: Int, flags: CMBlockBufferFlags) -> OSStatus

Adds a reference to an existing block buffer.

func CMBlockBufferAssureBlockMemory(CMBlockBuffer) -> OSStatus

Assures that the system allocates memory for all memory blocks in a block buffer.

func CMBlockBufferAccessDataBytes(CMBlockBuffer, atOffset: Int, length: Int, temporaryBlock: UnsafeMutableRawPointer, returnedPointerOut: UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;CChar>?>) -> OSStatus

Accesses potentially noncontiguous data in a block buffer.

func CMBlockBufferCopyDataBytes(CMBlockBuffer, atOffset: Int, dataLength: Int, destination: UnsafeMutableRawPointer) -> OSStatus

Copies bytes from a block buffer into a provided memory area.

func CMBlockBufferReplaceDataBytes(with: UnsafeRawPointer, blockBuffer: CMBlockBuffer, offsetIntoDestination: Int, dataLength: Int) -> OSStatus

Copies bytes from a given memory block into a block buffer replacing bytes in the underlying data blocks.

func CMBlockBufferFillDataBytes(with: CChar, blockBuffer: CMBlockBuffer, offsetIntoDestination: Int, dataLength: Int) -> OSStatus

Fills the destination buffer with the specified data byte.

### Inspecting a Block Buffer

func CMBlockBufferGetDataPointer(CMBlockBuffer, atOffset: Int, lengthAtOffsetOut: UnsafeMutablePointer&lt;Int>?, totalLengthOut: UnsafeMutablePointer&lt;Int>?, dataPointerOut: UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;CChar>?>?) -> OSStatus

Gains access to the data represented by a block buffer.

func CMBlockBufferGetDataLength(CMBlockBuffer) -> Int

Returns the total length of data that’s accessible by a block buffer.

func CMBlockBufferIsRangeContiguous(CMBlockBuffer, atOffset: Int, length: Int) -> Bool

Returns a Boolean value that indicates whether the specified range within a block buffer is contiguous.

func CMBlockBufferIsEmpty(CMBlockBuffer) -> Bool

Returns a Boolean value that indicates whether the buffer is empty.

### Accessing the Type Identifier

func CMBlockBufferGetTypeID() -> CFTypeID

Returns the type identifier for block buffer objects.

### Data Types

class CMBlockBuffer

A reference to a block buffer instance.

protocol CMBlockBufferProtocol

A protocol for objects that operate on a range of a block buffer.

### Errors

Block Buffer Error Codes

Error codes that framework operations produce.

## See Also

### Sample Processing

CMSampleBuffer APIs

An object that contains zero or more media samples of a uniform media type.

struct CMTaggedBuffer

An instance of a media buffer containing metadata tags.

CMTaggedBufferGroup APIs

Objective-C types and interfaces for working with Core Media tagged buffer groups.

CMFormatDescription APIs

A media format descriptor that describes the samples in a sample buffer.

CMAttachment APIs

Add supporting metadata to sample buffers.

