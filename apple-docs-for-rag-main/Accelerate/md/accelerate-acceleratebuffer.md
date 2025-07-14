

- Accelerate
-  AccelerateBuffer 

Protocol

# AccelerateBuffer

A type that represents an immutable buffer.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
protocol AccelerateBuffer
```

## Overview

If you implement your own type that conforms to AccelerateBuffer and uses the default implementation of withUnsafeBufferPointer(_:), your type needs to return a nonnil result from withContiguousStorageIfAvailable(_:).

## Topics

### Associated Types

associatedtype Element

The buffer’s element type.

**Required**

### Instance Properties

var count: Int

The number of elements in the buffer.

**Required**

### Instance Methods

func withUnsafeBufferPointer&lt;R>((UnsafeBufferPointer&lt;Self.Element>) throws -> R) rethrows -> R

Calls a closure with a pointer to the object’s contiguous storage.

**Required** Default implementation provided.

## Relationships

### Inherited By

- AccelerateMutableBuffer

### Conforming Types

- vImage.PixelBuffer

  Conforms when `Format` conforms to `StaticPixelFormat`.

## See Also

### Essentials

protocol AccelerateMutableBuffer

A type that represents a mutable buffer.

protocol AccelerateMatrixBuffer

protocol AccelerateMutableMatrixBuffer

enum AccelerateMatrixOrder

