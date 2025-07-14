

- Media Player
-  MPSkipIntervalCommandEvent 

Class

# MPSkipIntervalCommandEvent

An event requesting a change in the current skip interval.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.12.2+tvOS 7.1+visionOS 1.0+watchOS 5.0+

``` source
class MPSkipIntervalCommandEvent
```

## Topics

### Retrieving the skip interval

var interval: TimeInterval

The chosen interval, in seconds, for the skip command event.

## Relationships

### Inherits From

- MPRemoteCommandEvent

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Responding to track navigation events

class MPChangePlaybackPositionCommand

An object that responds to requests to change the current playback position of the playing item.

class MPChangePlaybackPositionCommandEvent

An event requesting a change in the playback position.

class MPSeekCommandEvent

An event requesting that the player seek to a new position.

class MPSkipIntervalCommand

An object that defines the skip intervals for the player.

