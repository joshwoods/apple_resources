

- AVFoundation
- AVVideoComposition
-  animationTool 

Instance Property

# animationTool

A video composition tool to use with Core Animation in offline rendering.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var animationTool: AVVideoCompositionCoreAnimationTool? { get }
```

## Discussion

This attribute may be `nil`. Set an animation tool if you’re using the composition in conjunction with AVAssetExportSession for offline rendering, rather than with AVPlayer.

## See Also

### Inspecting the Video Composition

var renderSize: CGSize

The size at which the video composition should render.

var renderScale: Float

The scale at which the video composition should render.

var frameDuration: CMTime

A time interval for which the video composition should render composed video frames.

var colorPrimaries: String?

The color primaries used for video composition.

var colorTransferFunction: String?

The transfer function used for video composition.

var colorYCbCrMatrix: String?

The YCbCr matrix used for video composition.

var customVideoCompositorClass: (any AVVideoCompositing.Type)?

A custom compositor class to use.

