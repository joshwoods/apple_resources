

- Accelerate
-  PixelFormat 

Protocol

# PixelFormat

A pixel buffer pixel format.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
protocol PixelFormat
```

## Topics

### Associated Types

associatedtype ComponentType : Equatable

The type of the pixel’s component.

**Required**

## Relationships

### Inherited By

- InitializableFromCGImage
- MultiplePlanePixelFormat
- SinglePlanePixelFormat
- StaticPixelFormat

### Conforming Types

- vImage.DynamicPixelFormat
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
- vImage.Planar8x2
- vImage.Planar8x3
- vImage.Planar8x4
- vImage.PlanarF
- vImage.PlanarFx2
- vImage.PlanarFx3
- vImage.PlanarFx4

## See Also

### Protocols

protocol StaticPixelFormat

A pixel format that’s known at compile time.

protocol InitializableFromCGImage

A pixel format that supports initialization from a Core Graphics image.

protocol SinglePlanePixelFormat

A pixel format that contains a single underlying vImage buffer.

protocol MultiplePlanePixelFormat

A pixel format that contains multiple homogeneous planes represented by multiple underlying vImage buffers.

