

- Accelerate
-  InitializableFromCGImage 

Protocol

# InitializableFromCGImage

A pixel format that supports initialization from a Core Graphics image.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
protocol InitializableFromCGImage : SinglePlanePixelFormat
```

## Topics

### Type Properties

static var bitCountPerComponent: Int

The number of bits in a channel.

**Required**

## Relationships

### Inherits From

- PixelFormat
- SinglePlanePixelFormat

### Conforming Types

- vImage.Interleaved16Fx4
- vImage.Interleaved16Ux2
- vImage.Interleaved16Ux4
- vImage.Interleaved8x3
- vImage.Interleaved8x4
- vImage.InterleavedFx3
- vImage.InterleavedFx4
- vImage.Planar16F
- vImage.Planar8
- vImage.PlanarF

## See Also

### Protocols

protocol PixelFormat

A pixel buffer pixel format.

protocol StaticPixelFormat

A pixel format that’s known at compile time.

protocol SinglePlanePixelFormat

A pixel format that contains a single underlying vImage buffer.

protocol MultiplePlanePixelFormat

A pixel format that contains multiple homogeneous planes represented by multiple underlying vImage buffers.

