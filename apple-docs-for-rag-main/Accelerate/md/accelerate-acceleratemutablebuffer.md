

- Accelerate
-  AccelerateMutableBuffer 

Protocol

# AccelerateMutableBuffer

A type that represents a mutable buffer.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
protocol AccelerateMutableBuffer : AccelerateBuffer
```

## Overview

If you implement your own type that conforms to AccelerateMutableBuffer and uses the default implementation of withUnsafeMutableBufferPointer(_:), your type needs to return a nonnil result from withContiguousMutableStorageIfAvailable(_:).

## Topics

### Instance Methods

func withUnsafeMutableBufferPointer&lt;R>((inout UnsafeMutableBufferPointer&lt;Self.Element>) throws -> R) rethrows -> R

Calls the given closure with a pointer to the object’s mutable contiguous storage.

**Required** Default implementation provided.

func withUnsafePixelBuffer&lt;R>(body: (vImage.PixelBuffer&lt;vImage.Planar16U>) throws -> R) rethrows -> R

func withUnsafePixelBuffer&lt;R>(body: (vImage.PixelBuffer&lt;vImage.Planar16F>) throws -> R) rethrows -> R

func withUnsafePixelBuffer&lt;R>(body: (vImage.PixelBuffer&lt;vImage.PlanarF>) throws -> R) rethrows -> R

func withUnsafePixelBuffer&lt;R>(body: (vImage.PixelBuffer&lt;vImage.Planar8>) throws -> R) rethrows -> R

## Relationships

### Inherits From

- AccelerateBuffer

### Conforming Types

- vImage.PixelBuffer

  Conforms when `Format` conforms to `StaticPixelFormat`.

## See Also

### Essentials

protocol AccelerateBuffer

A type that represents an immutable buffer.

protocol AccelerateMatrixBuffer

protocol AccelerateMutableMatrixBuffer

enum AccelerateMatrixOrder

