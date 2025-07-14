

- Foundation
-  ContiguousBytes 

Protocol

# ContiguousBytes

A protocol that declares the type offers direct access to the underlying raw bytes in a contiguous manner.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol ContiguousBytes
```

## Topics

### Accessing Underlying Storage

func withUnsafeBytes&lt;R>((UnsafeRawBufferPointer) throws -> R) rethrows -> R

Calls the given closure with a pointer to the underlying bytes of the type’s contiguous storage.

**Required**

## Relationships

### Conforming Types

- Data

## See Also

### Binary Data

struct Data

A byte buffer in memory.

protocol DataProtocol

A protocol that provides consistent data access to the bytes underlying contiguous and noncontiguous data buffers.

protocol MutableDataProtocol

A protocol that provides consistent data access to the bytes underlying contiguous and noncontiguous mutable data buffers.

