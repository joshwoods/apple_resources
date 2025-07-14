

- AVFoundation
- AVVideoCompositionRenderContext
-  renderTransform 

Instance Property

# renderTransform

A transform to apply to the source image.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var renderTransform: CGAffineTransform { get }
```

## Discussion

The transform to apply to the source image incorporating the renderScale, pixelAspectRatio, and edgeWidths.

The coordinate system origin is the top left corner of the buffer.

## See Also

### Getting the Render Settings

var videoComposition: AVVideoComposition

The video composition being rendered.

var highQualityRendering: Bool

The rendering quality to use.

var renderScale: Float

A scaling ratio that is applied when rendering frames.

var size: CGSize

The width and height for the rendering frames.

