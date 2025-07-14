

- Foundation
-  MutableDataProtocol 

Protocol

# MutableDataProtocol

A protocol that provides consistent data access to the bytes underlying contiguous and noncontiguous mutable data buffers.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol MutableDataProtocol : DataProtocol, MutableCollection, RangeReplaceableCollection
```

## Topics

### Resetting Backing Storage

func resetBytes&lt;R>(in: R)

Replaces the contents of the data buffer with zeros for the provided range.

**Required** Default implementation provided.

## Relationships

### Inherits From

- BidirectionalCollection
- Collection
- DataProtocol
- MutableCollection
- RandomAccessCollection
- RangeReplaceableCollection
- Sequence

### Conforming Types

- Data

## See Also

### Binary Data

struct Data

A byte buffer in memory.

protocol DataProtocol

A protocol that provides consistent data access to the bytes underlying contiguous and noncontiguous data buffers.

protocol ContiguousBytes

A protocol that declares the type offers direct access to the underlying raw bytes in a contiguous manner.

