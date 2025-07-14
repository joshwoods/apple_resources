

- Core Media
- CMBlockBuffer
-  append(bufferReference:flags:) 

Instance Method

# append(bufferReference:flags:)

Adds a reference to another block buffer.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func append(
    bufferReference: T,
    flags: CMBlockBuffer.Flags = []
) throws where T : CMBlockBufferProtocol
```

## Parameters 

`bufferReference`  

A block buffer to refer to. The buffer must not be empty unless you also pass the permitEmptyReference flag.

`flags`  

Feature and control flags.

## See Also

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

func assureBlockMemory() throws

Assures that the system allocates all memory blocks.

func withUnsafeMutableBytes&lt;R>(atOffset: Int, (UnsafeMutableRawBufferPointer) throws -> R) throws -> R

Accesses the data that a block buffer represents.

