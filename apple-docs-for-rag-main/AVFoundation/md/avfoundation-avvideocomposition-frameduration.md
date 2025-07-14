

- AVFoundation
- AVVideoComposition
-  frameDuration 

Instance Property

# frameDuration

A time interval for which the video composition should render composed video frames.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var frameDuration: CMTime { get }
```

## See Also

### Inspecting the Video Composition

var renderSize: CGSize

The size at which the video composition should render.

var renderScale: Float

The scale at which the video composition should render.

var animationTool: AVVideoCompositionCoreAnimationTool?

A video composition tool to use with Core Animation in offline rendering.

var colorPrimaries: String?

The color primaries used for video composition.

var colorTransferFunction: String?

The transfer function used for video composition.

var colorYCbCrMatrix: String?

The YCbCr matrix used for video composition.

var customVideoCompositorClass: (any AVVideoCompositing.Type)?

A custom compositor class to use.

