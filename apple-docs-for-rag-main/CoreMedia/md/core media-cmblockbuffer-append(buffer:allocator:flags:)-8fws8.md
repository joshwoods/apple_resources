

- Core Media
- CMBlockBuffer
-  append(buffer:allocator:flags:) 

Instance Method

# append(buffer:allocator:flags:)

Adds a sliced memory block to a block buffer using a custom allocator.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func append(
    buffer: Slice,
    allocator: CFAllocator? = kCFAllocatorDefault,
    flags: CMBlockBuffer.Flags = []
) throws
```

## Parameters 

`buffer`  

A block of memory to hold buffered data.

`allocator`  

An allocator for the memory block.

`flags`  

Feature and control flags.

## See Also

### Modifying a Block Buffer

func append(length: Int, allocator: CFAllocator?, range: Range&lt;Int>?, flags: CMBlockBuffer.Flags) throws

Adds a memory block to an existing block buffer.

func append(buffer: UnsafeMutableRawBufferPointer, allocator: CFAllocator?, flags: CMBlockBuffer.Flags) throws

Adds a memory block to a block buffer using a custom allocator.

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

