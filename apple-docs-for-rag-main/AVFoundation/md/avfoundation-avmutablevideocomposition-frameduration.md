

- AVFoundation
- AVMutableVideoComposition
-  frameDuration 

Instance Property

# frameDuration

A time interval for which the video composition should render composed video frames.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var frameDuration: CMTime { get set }
```

## See Also

### Configuring Video Composition Properties

var renderSize: CGSize

The size at which the video composition should render.

var renderScale: Float

The scale at which the video composition should render.

var animationTool: AVVideoCompositionCoreAnimationTool?

A video composition tool to use with Core Animation in offline rendering.

