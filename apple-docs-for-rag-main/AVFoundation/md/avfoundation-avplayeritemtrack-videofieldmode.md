

- AVFoundation
- AVPlayerItemTrack
-  videoFieldMode 

Instance Property

# videoFieldMode

A mode that specifies the handling of video frames that contain multiple fields.

macOS 10.10+

``` source
nonisolated
var videoFieldMode: String? { get set }
```

## Discussion

A value of `nil` indicates default processing of video frames. To deinterlace video fields, set this property value to AVPlayerItemTrackVideoFieldModeDeinterlaceFields.

## See Also

### Configuring Video Properties

var currentVideoFrameRate: Float

The current frame rate of the video track as it plays.

let AVPlayerItemTrackVideoFieldModeDeinterlaceFields: String

A video field mode that requests deinterlacing of video fields.

