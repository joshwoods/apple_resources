

- AVFoundation
- AVVideoComposition
-  renderScale 

Instance Property

# renderScale

The scale at which the video composition should render.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.14+tvOS 9.0+visionOS 1.0+

``` source
var renderScale: Float { get }
```

## Discussion

This value must be `1.0` unless you set the composition on an AVPlayerItem.

## See Also

### Inspecting the Video Composition

var renderSize: CGSize

The size at which the video composition should render.

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

var customVideoCompositorClass: (any AVVideoCompositing.Type)?

A custom compositor class to use.

