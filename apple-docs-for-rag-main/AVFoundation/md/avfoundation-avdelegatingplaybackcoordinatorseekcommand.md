

- AVFoundation
-  AVDelegatingPlaybackCoordinatorSeekCommand 

Class

# AVDelegatingPlaybackCoordinatorSeekCommand

A command that indicates to seek to a new time in the item timeline.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
class AVDelegatingPlaybackCoordinatorSeekCommand
```

## Topics

### Accessing Command Details

var shouldBufferInAnticipationOfPlayback: Bool

A Boolean value that indicates whether the player starts buffering in anticipation of a request to begin playback.

var anticipatedPlaybackRate: Float

The rate at which the coordinator expects playback to resume.

var itemTime: CMTime

The time to seek to in the item timeline.

var completionDueDate: Date?

The deadline by which the coordinator expects the delegate to handle the command.

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

class AVDelegatingPlaybackCoordinatorPauseCommand

A command that indicates to pause playback.

class AVDelegatingPlaybackCoordinatorBufferingCommand

A command that indicates to start buffering data in preparation for playback.

