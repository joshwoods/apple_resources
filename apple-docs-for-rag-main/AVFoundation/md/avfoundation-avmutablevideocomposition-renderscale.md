

- AVFoundation
- AVMutableVideoComposition
-  renderScale 

Instance Property

# renderScale

The scale at which the video composition should render.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.14+tvOS 9.0+visionOS 1.0+

``` source
var renderScale: Float { get set }
```

## Discussion

May only be other than `1.0` for a video composition set on an AVPlayerItem.

## See Also

### Configuring Video Composition Properties

var frameDuration: CMTime

A time interval for which the video composition should render composed video frames.

var renderSize: CGSize

The size at which the video composition should render.

var animationTool: AVVideoCompositionCoreAnimationTool?

A video composition tool to use with Core Animation in offline rendering.

