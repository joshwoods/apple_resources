

- Foundation
-  DataProtocol 

Protocol

# DataProtocol

A protocol that provides consistent data access to the bytes underlying contiguous and noncontiguous data buffers.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol DataProtocol : RandomAccessCollection where Self.Element == UInt8, Self.SubSequence : DataProtocol
```

## Topics

### Accessing Backing Storage

var regions: Self.Regions

A collection of buffers that make up the whole of the type conforming to a data protocol.

**Required**

associatedtype Regions : BidirectionalCollection

A type that represents a collection of contiguous parts that make up the type conforming to a data protocol.

**Required**

### Copying Underlying Bytes

func copyBytes&lt;DestinationType>(to: UnsafeMutableBufferPointer&lt;DestinationType>) -> Int

Copies the bytes of data from the type into a typed memory buffer.

func copyBytes(to: UnsafeMutableRawBufferPointer) -> Int

Copies the bytes of data from the type into a raw memory buffer.

func copyBytes&lt;DestinationType>(to: UnsafeMutableBufferPointer&lt;DestinationType>, count: Int) -> Int

Copies the provided number of bytes from the start of the type into a typed memory buffer.

**Required** Default implementations provided.

func copyBytes(to: UnsafeMutableRawBufferPointer, count: Int) -> Int

Copies the provided number of bytes from the start of the type into a raw memory buffer.

**Required** Default implementations provided.

func copyBytes&lt;DestinationType, R>(to: UnsafeMutableBufferPointer&lt;DestinationType>, from: R) -> Int

Copies a range of the bytes from the type into a typed memory buffer.

**Required** Default implementations provided.

func copyBytes&lt;R>(to: UnsafeMutableRawBufferPointer, from: R) -> Int

Copies a range of the bytes from the type into a raw memory buffer.

**Required** Default implementations provided.

### Searching Within Data

func firstRange&lt;D>(of: D) -> Range&lt;Self.Index>?

Returns the first found range of the type’s data buffer.

func firstRange&lt;D, R>(of: D, in: R) -> Range&lt;Self.Index>?

Returns the first found range of the type’s data buffer.

**Required** Default implementation provided.

func lastRange&lt;D>(of: D) -> Range&lt;Self.Index>?

Returns the last found range of the type’s data buffer.

func lastRange&lt;D, R>(of: D, in: R) -> Range&lt;Self.Index>?

Returns the last found range of the type’s data buffer.

**Required** Default implementation provided.

## Relationships

### Inherits From

- BidirectionalCollection
- Collection
- RandomAccessCollection
- Sequence

### Inherited By

- MutableDataProtocol

### Conforming Types

- Data
- NSData
- NSMutableData
- NSPurgeableData

## See Also

### Binary Data

struct Data

A byte buffer in memory.

protocol MutableDataProtocol

A protocol that provides consistent data access to the bytes underlying contiguous and noncontiguous mutable data buffers.

protocol ContiguousBytes

A protocol that declares the type offers direct access to the underlying raw bytes in a contiguous manner.

