

- AVFoundation
- AVAssetExportSession
-  videoComposition 

Instance Property

# videoComposition

An optional object that provides instructions for how to composite frames of video.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
@NSCopying
var videoComposition: AVVideoComposition? { get set }
```

## Discussion

The default value is `nil`.

This property is key-value observable.

## See Also

### Configuring Video Output

var customVideoCompositor: (any AVVideoCompositing)?

An optional custom object to use when compositing video frames.

