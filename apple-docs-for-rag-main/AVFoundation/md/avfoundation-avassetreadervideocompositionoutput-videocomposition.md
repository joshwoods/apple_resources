

- AVFoundation
- AVAssetReaderVideoCompositionOutput
-  videoComposition 

Instance Property

# videoComposition

The video composition to use for the output.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
@NSCopying
var videoComposition: AVVideoComposition? { get set }
```

## Discussion

The value is an AVVideoComposition object that specifies the visual arrangement of video frames read from each source track over the timeline of the source asset.

## See Also

### Configuring Video Settings

var customVideoCompositor: (any AVVideoCompositing)?

A custom video compositor for the output.

