

- Core Media
-  CMBlockBufferProtocol 

Protocol

# CMBlockBufferProtocol

A protocol for objects that operate on a range of a block buffer.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol CMBlockBufferProtocol
```

## Topics

### Modifying a Block Buffer

func copyDataBytes(to: UnsafeMutableRawBufferPointer) throws

func dataBytes() throws -> Data

func fillDataBytes(with: UInt8) throws

func replaceDataBytes(with: UnsafeRawBufferPointer) throws

var isContiguous: Bool

func makeContiguous(allocator: CMBlockBuffer.CustomBlockAllocator, deallocator: CMBlockBuffer.CustomBlockDeallocator, flags: CMBlockBuffer.Flags) throws -> CMBlockBuffer

func makeContiguous(allocator: CFAllocator?, flags: CMBlockBuffer.Flags) throws -> CMBlockBuffer

func withContiguousStorage&lt;R>((UnsafeRawBufferPointer) throws -> R) throws -> R

### Inspecting a Block Buffer

var dataLength: Int

var startIndex: Int

**Required**

var endIndex: Int

**Required**

var owner: CMBlockBuffer

**Required**

### Subscripts

subscript(ClosedRange&lt;Int>) -> CMBlockBuffer.Slice

Creates a slice from a `ClosedRange`.

subscript(Range&lt;Int>) -> CMBlockBuffer.Slice

subscript(PartialRangeFrom&lt;Int>) -> CMBlockBuffer.Slice

subscript(PartialRangeUpTo&lt;Int>) -> CMBlockBuffer.Slice

subscript(PartialRangeThrough&lt;Int>) -> CMBlockBuffer.Slice

subscript((UnboundedRange_) -> ()) -> CMBlockBuffer.Slice

## Relationships

### Conforming Types

- CMBlockBuffer
- CMBlockBuffer.Slice

## See Also

### Data Types

class CMBlockBuffer

A reference to a block buffer instance.

