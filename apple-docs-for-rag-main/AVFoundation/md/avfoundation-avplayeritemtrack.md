

- AVFoundation
-  AVPlayerItemTrack 

Class

# AVPlayerItemTrack

An object that represents the presentation state of an asset track during playback.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
@MainActor
class AVPlayerItemTrack
```

## Topics

### Setting the Enabled State

var isEnabled: Bool

A Boolean value that indicates whether the player item presents the track’s media during playback.

### Configuring Video Properties

var currentVideoFrameRate: Float

The current frame rate of the video track as it plays.

var videoFieldMode: String?

A mode that specifies the handling of video frames that contain multiple fields.

let AVPlayerItemTrackVideoFieldModeDeinterlaceFields: String

A video field mode that requests deinterlacing of video fields.

### Accessing the Asset Track

var assetTrack: AVAssetTrack?

An asset track that provides the media for the player item track.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Playback control

Controlling the transport behavior of a player

Play, pause, and seek through a media presentation.

class AVPlayer

An object that provides the interface to control the player’s transport behavior.

class AVPlayerItem

An object that models the timing and presentation state of an asset during playback.

class AVQueuePlayer

An object that plays a sequence of player items.

class AVPlayerLooper

An object that loops media content using a queue player.

