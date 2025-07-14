

- Accelerate
-  AccelerateMutableMatrixBuffer 

Protocol

# AccelerateMutableMatrixBuffer

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOSwatchOS 11.0+

``` source
protocol AccelerateMutableMatrixBuffer : AccelerateMatrixBuffer
```

## Topics

### Instance Methods

func withUnsafeMutableBufferPointer&lt;R>((inout UnsafeMutableBufferPointer&lt;Self.Element>) throws -> R) rethrows -> R

**Required**

## Relationships

### Inherits From

- AccelerateMatrixBuffer

### Conforming Types

- vImage.PixelBuffer

  Conforms when `Format` conforms to `StaticPixelFormat`.

## See Also

### Essentials

protocol AccelerateBuffer

A type that represents an immutable buffer.

protocol AccelerateMutableBuffer

A type that represents a mutable buffer.

protocol AccelerateMatrixBuffer

enum AccelerateMatrixOrder

