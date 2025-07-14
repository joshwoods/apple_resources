

- Accelerate
-  StaticPixelFormat 

Protocol

# StaticPixelFormat

A pixel format that’s known at compile time.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
protocol StaticPixelFormat : SinglePlanePixelFormat
```

## Topics

### Type Properties

static var bitCountPerPixel: Int

The number of bits allocated for a single pixel.

**Required**

static var channelCount: Int

The number of channels in a pixel buffer.

**Required**

## Relationships

### Inherits From

- PixelFormat
- SinglePlanePixelFormat

### Conforming Types

- vImage.Interleaved16Fx2
- vImage.Interleaved16Fx4
- vImage.Interleaved16Ux2
- vImage.Interleaved16Ux4
- vImage.Interleaved8x2
- vImage.Interleaved8x3
- vImage.Interleaved8x4
- vImage.InterleavedFx2
- vImage.InterleavedFx3
- vImage.InterleavedFx4
- vImage.Planar16F
- vImage.Planar16U
- vImage.Planar8
- vImage.PlanarF

## See Also

### Protocols

protocol PixelFormat

A pixel buffer pixel format.

protocol InitializableFromCGImage

A pixel format that supports initialization from a Core Graphics image.

protocol SinglePlanePixelFormat

A pixel format that contains a single underlying vImage buffer.

protocol MultiplePlanePixelFormat

A pixel format that contains multiple homogeneous planes represented by multiple underlying vImage buffers.

