

- AVFoundation
- AVPlayerItem
-  videoComposition 

Instance Property

# videoComposition

The video composition settings to be applied during playback.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var videoComposition: AVVideoComposition? { get set }
```

## Discussion

A video composition can only be used with file-based media and is not supported for use with media served using HTTP Live Streaming.

## See Also

### Configuring Video Compositing

var customVideoCompositor: (any AVVideoCompositing)?

The custom video compositor.

var seekingWaitsForVideoCompositionRendering: Bool

A Boolean value that indicates whether the item’s timing follows the displayed video frame when seeking with a video composition.

