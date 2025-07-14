

- AVFoundation
- AVVideoCompositionRenderContext
-  highQualityRendering 

Instance Property

# highQualityRendering

The rendering quality to use.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var highQualityRendering: Bool { get }
```

## Discussion

Specifies that the custom compositor should use higher quality, potentially slower algorithms.

Generally this property is true for non-real-time use cases.

## See Also

### Getting the Render Settings

var videoComposition: AVVideoComposition

The video composition being rendered.

var renderScale: Float

A scaling ratio that is applied when rendering frames.

var renderTransform: CGAffineTransform

A transform to apply to the source image.

var size: CGSize

The width and height for the rendering frames.

