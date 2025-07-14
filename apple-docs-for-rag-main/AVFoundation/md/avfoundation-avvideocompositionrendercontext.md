

- AVFoundation
-  AVVideoCompositionRenderContext 

Class

# AVVideoCompositionRenderContext

An object that defines the context in which custom compositors render pixel buffers.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
class AVVideoCompositionRenderContext
```

## Overview

A render context provides size and scaling information and offers a service for efficiently providing pixel buffers from a managed pool of buffers.

## Topics

### Creating the Pixel Buffer

func newPixelBuffer() -> CVPixelBuffer?

Returns a pixel buffer to use for rendering.

### Getting the Render Settings

var videoComposition: AVVideoComposition

The video composition being rendered.

var highQualityRendering: Bool

The rendering quality to use.

var renderScale: Float

A scaling ratio that is applied when rendering frames.

var renderTransform: CGAffineTransform

A transform to apply to the source image.

var size: CGSize

The width and height for the rendering frames.

### Getting Pixel and Edge Width Information

var edgeWidths: AVEdgeWidths

The width of the edge processing region on the left, top, right, and bottom edges, in pixels.

struct AVEdgeWidths

A structure that defines edge processing region widths.

var pixelAspectRatio: AVPixelAspectRatio

The pixel aspect ratio for rendered frames.

struct AVPixelAspectRatio

A structure that defines a pixel aspect ratio for a rendering context.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Observing Render Context Changes

func renderContextChanged(AVVideoCompositionRenderContext)

Tells the compositor that the composition changed render contexts.

**Required**

