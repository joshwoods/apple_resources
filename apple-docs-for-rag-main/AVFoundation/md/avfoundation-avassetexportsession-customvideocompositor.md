

- AVFoundation
- AVAssetExportSession
-  customVideoCompositor 

Instance Property

# customVideoCompositor

An optional custom object to use when compositing video frames.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var customVideoCompositor: (any AVVideoCompositing)? { get }
```

## See Also

### Configuring Video Output

var videoComposition: AVVideoComposition?

An optional object that provides instructions for how to composite frames of video.

