

- Core Media
- CMBlockBufferProtocol
-  makeContiguous(allocator:deallocator:flags:) 

Instance Method

# makeContiguous(allocator:deallocator:flags:)

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func makeContiguous(
    allocator: @escaping CMBlockBuffer.CustomBlockAllocator,
    deallocator: @escaping CMBlockBuffer.CustomBlockDeallocator,
    flags: CMBlockBuffer.Flags = []
) throws -> CMBlockBuffer
```

## See Also

### Modifying a Block Buffer

func copyDataBytes(to: UnsafeMutableRawBufferPointer) throws

func dataBytes() throws -> Data

func fillDataBytes(with: UInt8) throws

func replaceDataBytes(with: UnsafeRawBufferPointer) throws

var isContiguous: Bool

func makeContiguous(allocator: CFAllocator?, flags: CMBlockBuffer.Flags) throws -> CMBlockBuffer

func withContiguousStorage&lt;R>((UnsafeRawBufferPointer) throws -> R) throws -> R

