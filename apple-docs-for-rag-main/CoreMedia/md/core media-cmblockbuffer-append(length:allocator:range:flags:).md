

- Core Media
- CMBlockBuffer
-  append(length:allocator:range:flags:) 

Instance Method

# append(length:allocator:range:flags:)

Adds a memory block to an existing block buffer.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func append(
    length: Int,
    allocator: CFAllocator? = kCFAllocatorDefault,
    range: Range? = nil,
    flags: CMBlockBuffer.Flags = []
) throws
```

## Parameters 

`length`  

The length of the memory block in bytes. Must not be zero. This is the size to allocate when you call the assureBlockMemory() function.

`allocator`  

The allocator to use to allocate the memory block.

`range`  

The range within the memory block to which the block buffer should refer to data. If this value is `nil`, the block buffer uses the whole memory block.

`flags`  

Flags to control the behavior of the operation.

## See Also

### Modifying a Block Buffer

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

