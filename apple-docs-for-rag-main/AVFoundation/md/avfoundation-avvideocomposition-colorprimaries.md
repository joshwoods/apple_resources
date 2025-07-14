

- AVFoundation
- AVVideoComposition
-  colorPrimaries 

Instance Property

# colorPrimaries

The color primaries used for video composition.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var colorPrimaries: String? { get }
```

## Discussion

The default value is `nil`. When the value of this property is `nil`, the source’s color primaries are propagated and used. Valid values are those suitable for AVVideoColorPrimariesKey.

## See Also

### Inspecting the Video Composition

var renderSize: CGSize

The size at which the video composition should render.

var renderScale: Float

The scale at which the video composition should render.

var frameDuration: CMTime

A time interval for which the video composition should render composed video frames.

var animationTool: AVVideoCompositionCoreAnimationTool?

A video composition tool to use with Core Animation in offline rendering.

var colorTransferFunction: String?

The transfer function used for video composition.

var colorYCbCrMatrix: String?

The YCbCr matrix used for video composition.

var customVideoCompositorClass: (any AVVideoCompositing.Type)?

A custom compositor class to use.

