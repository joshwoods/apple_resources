

- AVFoundation
- AVVideoComposition
-  customVideoCompositorClass 

Instance Property

# customVideoCompositorClass

A custom compositor class to use.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var customVideoCompositorClass: (any AVVideoCompositing.Type)? { get }
```

## Discussion

The default is `nil`, which indicates to use the internal video compositor. The `customVideoCompositorClass` must implement the AVVideoCompositing protocol.

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

var colorPrimaries: String?

The color primaries used for video composition.

var colorTransferFunction: String?

The transfer function used for video composition.

var colorYCbCrMatrix: String?

The YCbCr matrix used for video composition.

