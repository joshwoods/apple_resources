

- Accelerate
-  MultiplePlanePixelFormat 

Protocol

# MultiplePlanePixelFormat

A pixel format that contains multiple homogeneous planes represented by multiple underlying vImage buffers.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
protocol MultiplePlanePixelFormat : PixelFormat
```

## Overview

Use multiple-plane pixel buffers to store image data as discrete planar buffers that represent individual channels.

For example, the following code deinterleaves an interleaved buffer and applies different gamma adjustments to different color channels. The code calls `PixelBuffer.convert(to:)` to reinterleave the image data and generates a CGImage instance of the final output.

```
let srcImage =  imageLiteral(resourceName: "...").cgImage(
    forProposedRect: nil,
    context: nil,
    hints: nil)!

var cgImageFormat = vImage_CGImageFormat(
    bitsPerComponent: 8,
    bitsPerPixel: 8 * 3,
    colorSpace: CGColorSpaceCreateDeviceRGB(),
    bitmapInfo: CGBitmapInfo(rawValue: CGImageAlphaInfo.none.rawValue))!

let interleaved = try vImage.PixelBuffer(
    cgImage: srcImage,
    cgImageFormat: &cgImageFormat,
    pixelFormat: vImage.Interleaved8x3.self)

let multiplane = vImage.PixelBuffer(interleavedBuffer: interleaved)

multiplane.withUnsafePixelBuffers { pixelBuffers in

    // Apply gamma to red channel.
    pixelBuffers[0].applyGamma(.nineOverElevenHalfPrecision,
                               destination: pixelBuffers[0])

    // Apply gamma to green channel.
    pixelBuffers[1].applyGamma(.fiveOverElevenHalfPrecision,
                               destination: pixelBuffers[1])
}

multiplane.convert(to: interleaved)
let outputImage = interleaved
```

## Topics

### Associated Types

associatedtype PlanarPixelFormat : StaticPixelFormat

**Required**

### Type Properties

static var bitCountPerPlanarPixel: Int

**Required**

static var planeCount: Int

**Required**

## Relationships

### Inherits From

- PixelFormat

### Conforming Types

- vImage.Planar8x2
- vImage.Planar8x3
- vImage.Planar8x4
- vImage.PlanarFx2
- vImage.PlanarFx3
- vImage.PlanarFx4

## See Also

### Protocols

protocol PixelFormat

A pixel buffer pixel format.

protocol StaticPixelFormat

A pixel format that’s known at compile time.

protocol InitializableFromCGImage

A pixel format that supports initialization from a Core Graphics image.

protocol SinglePlanePixelFormat

A pixel format that contains a single underlying vImage buffer.

