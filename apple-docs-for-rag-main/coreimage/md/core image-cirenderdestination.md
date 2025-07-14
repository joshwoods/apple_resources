

- Core Image
-  CIRenderDestination 

Class

# CIRenderDestination

A specification for configuring all attributes of a render task's destination and issuing asynchronous render tasks.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class CIRenderDestination : NSObject
```

## Overview

The `CIRenderDestination` class provides an API for specifying a render task destination's properties, such as buffer format, alpha mode, clamping behavior, blending, and color space, properties formerly tied to CIContext.

You can create a `CIRenderDestination` object for each surface or buffer to which you must render. You can also render multiple times to a single destination with different settings such as colorspace and blend mode by mutating a single `CIRenderDestination` object between renders.

Renders issued to a `CIRenderDestination` return to the caller as soon as the CPU has issued the task, rather than after the GPU has performed the task, so you can start render tasks on subsequent frames without waiting for previous renders to finish. If the render fails, a CIRenderTask will return immediately.

## Topics

### Creating a Render Destination

init(pixelBuffer: CVPixelBuffer)

Creates a render destination based on a Core Video pixel buffer.

init(ioSurface: IOSurface)

Creates a render destination based on an IOSurface object.

init(mtlTexture: any MTLTexture, commandBuffer: (any MTLCommandBuffer)?)

Creates a render destination based on a Metal texture.

init(width: Int, height: Int, pixelFormat: MTLPixelFormat, commandBuffer: (any MTLCommandBuffer)?, mtlTextureProvider: (() -> any MTLTexture)?)

Creates a render destination based on a Metal texture with specified pixel format.

init(glTexture: UInt32, target: UInt32, width: Int, height: Int)

Creates a render destination based on an OpenGL texture.

init(bitmapData: UnsafeMutableRawPointer, width: Int, height: Int, bytesPerRow: Int, format: CIFormat)

Creates a render destination based on a client-managed buffer.

### Customizing Rendering

var alphaMode: CIRenderDestinationAlphaMode

The render destination's representation of alpha (transparency) values.

enum CIRenderDestinationAlphaMode

Different ways of representing alpha.

var blendKernel: CIBlendKernel?

The destination's blend kernel.

var blendsInDestinationColorSpace: Bool

Indicator of whether to blend in the destination's color space.

var colorSpace: CGColorSpace?

The destination's color space.

var width: Int

The render destination's row width.

var height: Int

The render destination's buffer height.

var isClamped: Bool

Indicator of whether or not the destination clamps.

var isDithered: Bool

Indicator of whether or not the destination dithers.

var isFlipped: Bool

Indicator of whether the destination is flipped.

## Relationships

### Inherits From

- NSObject

## See Also

### Custom Render Destination

Generating an animation with a Core Image Render Destination

Animate a filtered image to a Metal view in a SwiftUI app using a Core Image Render Destination.

class CIRenderInfo

An encapsulation of a render task's timing, passes, and pixels processed.

class CIRenderTask

A single render task issued in conjunction with CIRenderDestination.

enum CIRenderDestinationAlphaMode

Different ways of representing alpha.

