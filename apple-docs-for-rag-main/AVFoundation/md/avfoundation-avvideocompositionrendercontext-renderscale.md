

- AVFoundation
- AVVideoCompositionRenderContext
-  renderScale 

Instance Property

# renderScale

A scaling ratio that is applied when rendering frames.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var renderScale: Float { get }
```

## See Also

### Getting the Render Settings

var videoComposition: AVVideoComposition

The video composition being rendered.

var highQualityRendering: Bool

The rendering quality to use.

var renderTransform: CGAffineTransform

A transform to apply to the source image.

var size: CGSize

The width and height for the rendering frames.

