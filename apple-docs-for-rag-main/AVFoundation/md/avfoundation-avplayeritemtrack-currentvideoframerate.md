

- AVFoundation
- AVPlayerItemTrack
-  currentVideoFrameRate 

Instance Property

# currentVideoFrameRate

The current frame rate of the video track as it plays.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
nonisolated
var currentVideoFrameRate: Float { get }
```

## Discussion

If the media type of the assetTrack is video, the property indicates the current frame rate of the track as it plays, in frames per second. If the item isn’t playing, or if the media type of the track isn’t video, the value of this property is `0.0`.

This property isn’t key-value observable.

## See Also

### Configuring Video Properties

var videoFieldMode: String?

A mode that specifies the handling of video frames that contain multiple fields.

let AVPlayerItemTrackVideoFieldModeDeinterlaceFields: String

A video field mode that requests deinterlacing of video fields.

