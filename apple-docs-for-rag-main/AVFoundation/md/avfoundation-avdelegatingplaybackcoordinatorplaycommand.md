

- AVFoundation
-  AVDelegatingPlaybackCoordinatorPlayCommand 

Class

# AVDelegatingPlaybackCoordinatorPlayCommand

A command that indicates to play at a specific rate and time.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
class AVDelegatingPlaybackCoordinatorPlayCommand
```

## Topics

### Accessing Command Details

var rate: Float

A rate to use when starting playback.

var itemTime: CMTime

A time in the item timeline to use to begin playback.

var hostClockTime: CMTime

A host clock time to use to begin playback.

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

class AVDelegatingPlaybackCoordinatorPauseCommand

A command that indicates to pause playback.

class AVDelegatingPlaybackCoordinatorSeekCommand

A command that indicates to seek to a new time in the item timeline.

class AVDelegatingPlaybackCoordinatorBufferingCommand

A command that indicates to start buffering data in preparation for playback.

