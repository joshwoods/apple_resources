

- AVFoundation
- AVPlayerItem
-  preferredMaximumResolution 

Instance Property

# preferredMaximumResolution

The desired maximum resolution of a video that is to be downloaded.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
nonisolated
var preferredMaximumResolution: CGSize { get set }
```

## Discussion

Defaults to CGSizeZero, which indicates there is no limit on the video resolution. Any other value indicates a preferred maximum video resolution. This property only applies to HTTP Live Streaming assets.

## See Also

### Configuring Presentation

var presentationSize: CGSize

The size at which the visual portion of the item is presented by the player.

var videoApertureMode: AVVideoApertureMode

The video aperture mode to apply during playback.

struct AVVideoApertureMode

A value that describes how a video is scaled or cropped.

