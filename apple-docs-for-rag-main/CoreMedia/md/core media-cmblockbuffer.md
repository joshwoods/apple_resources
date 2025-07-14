

- Core Media
-  CMBlockBuffer 

Class

# CMBlockBuffer

A reference to a block buffer instance.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
class CMBlockBuffer
```

## Topics

### Modifying a Block Buffer

func append(length: Int, allocator: CFAllocator?, range: Range&lt;Int>?, flags: CMBlockBuffer.Flags) throws

Adds a memory block to an existing block buffer.

func append(buffer: UnsafeMutableRawBufferPointer, allocator: CFAllocator?, flags: CMBlockBuffer.Flags) throws

Adds a memory block to a block buffer using a custom allocator.

func append(buffer: Slice&lt;UnsafeMutableRawBufferPointer>, allocator: CFAllocator?, flags: CMBlockBuffer.Flags) throws

Adds a sliced memory block to a block buffer using a custom allocator.

func append(length: Int, allocator: CMBlockBuffer.CustomBlockAllocator, deallocator: CMBlockBuffer.CustomBlockDeallocator, range: Range&lt;Int>?, flags: CMBlockBuffer.Flags) throws

Adds a memory block to a block buffer using a custom allocator and deallocator.

func append(buffer: UnsafeMutableRawBufferPointer, deallocator: CMBlockBuffer.CustomBlockDeallocator, flags: CMBlockBuffer.Flags) throws

Adds a memory block to a block buffer with a custom deallocator.

func append(buffer: Slice&lt;UnsafeMutableRawBufferPointer>, deallocator: CMBlockBuffer.CustomBlockDeallocator, flags: CMBlockBuffer.Flags) throws

Adds a sliced memory block to a block buffer with a custom deallocator.

typealias CustomBlockAllocator

A type that allocates memory blocks.

typealias CustomBlockDeallocator

A type that deallocates memory blocks.

func append&lt;T>(bufferReference: T, flags: CMBlockBuffer.Flags) throws

Adds a reference to another block buffer.

func assureBlockMemory() throws

Assures that the system allocates all memory blocks.

func withUnsafeMutableBytes&lt;R>(atOffset: Int, (UnsafeMutableRawBufferPointer) throws -> R) throws -> R

Accesses the data that a block buffer represents.

### Inspecting a Block Buffer

var isEmpty: Bool

A Boolean value that indicates whether the block buffer is empty.

### Accessing the Type Identifier

class var typeID: CFTypeID

The type identifier for block buffer objects.

### Data Types

struct Error

A structure that defines block buffer errors.

struct Flags

A structure that defines feature and control flags.

struct Slice

A structure that defines a slice of a block buffer.

## Relationships

### Conforms To

- CMAttachmentBearerProtocol
- CMBlockBufferProtocol
- Copyable
- Equatable
- Hashable

## See Also

### Data Types

protocol CMBlockBufferProtocol

A protocol for objects that operate on a range of a block buffer.

