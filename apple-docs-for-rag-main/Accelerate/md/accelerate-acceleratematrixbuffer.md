

- Accelerate
-  AccelerateMatrixBuffer 

Protocol

# AccelerateMatrixBuffer

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOSwatchOS 11.0+

``` source
protocol AccelerateMatrixBuffer
```

## Topics

### Associated Types

associatedtype Element

**Required**

### Instance Properties

var accelerateMatrixOrder: AccelerateMatrixOrder

**Required**

var columnCount: Int

**Required**

var leadingDimension: Int

**Required**

var rowCount: Int

**Required**

### Instance Methods

func withUnsafeBufferPointer&lt;R>((UnsafeBufferPointer&lt;Self.Element>) throws -> R) rethrows -> R

**Required**

## Relationships

### Inherited By

- AccelerateMutableMatrixBuffer

### Conforming Types

- vImage.PixelBuffer

  Conforms when `Format` conforms to `StaticPixelFormat`.

## See Also

### Essentials

protocol AccelerateBuffer

A type that represents an immutable buffer.

protocol AccelerateMutableBuffer

A type that represents a mutable buffer.

protocol AccelerateMutableMatrixBuffer

enum AccelerateMatrixOrder

