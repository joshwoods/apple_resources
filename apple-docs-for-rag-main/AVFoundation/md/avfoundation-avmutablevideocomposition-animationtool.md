

- AVFoundation
- AVMutableVideoComposition
-  animationTool 

Instance Property

# animationTool

A video composition tool to use with Core Animation in offline rendering.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var animationTool: AVVideoCompositionCoreAnimationTool? { get set }
```

## Discussion

This attribute may be `nil`. Set an animation tool if you are using the composition in conjunction with AVAssetExportSession for offline rendering, rather than with AVPlayer.

## See Also

### Configuring Video Composition Properties

var frameDuration: CMTime

A time interval for which the video composition should render composed video frames.

var renderSize: CGSize

The size at which the video composition should render.

var renderScale: Float

The scale at which the video composition should render.

