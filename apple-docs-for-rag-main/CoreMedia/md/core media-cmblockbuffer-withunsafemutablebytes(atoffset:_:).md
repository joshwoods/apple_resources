

- Core Media
- CMBlockBuffer
-  withUnsafeMutableBytes(atOffset:\_:) 

Instance Method

# withUnsafeMutableBytes(atOffset:\_:)

Accesses the data that a block buffer represents.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func withUnsafeMutableBytes(
    atOffset offset: Int = 0,
    _ body: (UnsafeMutableRawBufferPointer) throws -> R
) throws -> R
```

## Parameters 

`offset`  

An offset within the buffer’s offset range.

`body`  

A closure the system calls with an UnsafeMutableRawBufferPointer parameter that points to contiguous storage in the block buffer.

## Return Value

The value, if any, that the body parameter returns

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

func append&lt;T>(bufferReference: T, flags: CMBlockBuffer.Flags) throws

Adds a reference to another block buffer.

func assureBlockMemory() throws

Assures that the system allocates all memory blocks.

