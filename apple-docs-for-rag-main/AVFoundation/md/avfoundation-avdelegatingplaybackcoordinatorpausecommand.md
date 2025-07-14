

- AVFoundation
-  AVDelegatingPlaybackCoordinatorPauseCommand 

Class

# AVDelegatingPlaybackCoordinatorPauseCommand

A command that indicates to pause playback.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
class AVDelegatingPlaybackCoordinatorPauseCommand
```

## Topics

### Accessing Command Details

var shouldBufferInAnticipationOfPlayback: Bool

A Boolean value that indicates whether the player starts buffering in preparation for a request to begin playback.

var anticipatedPlaybackRate: Float

The rate at which the coordinator expects the current item to play.

## Relationships

### Inherits From

- AVDelegatingPlaybackCoordinatorPlaybackControlCommand

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Playback Commands

class AVDelegatingPlaybackCoordinatorPlaybackControlCommand

An abstract superclass for playback commands.

class AVDelegatingPlaybackCoordinatorPlayCommand

A command that indicates to play at a specific rate and time.

class AVDelegatingPlaybackCoordinatorSeekCommand

A command that indicates to seek to a new time in the item timeline.

class AVDelegatingPlaybackCoordinatorBufferingCommand

A command that indicates to start buffering data in preparation for playback.

