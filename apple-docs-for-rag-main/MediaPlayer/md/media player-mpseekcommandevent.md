

- Media Player
-  MPSeekCommandEvent 

Class

# MPSeekCommandEvent

An event requesting that the player seek to a new position.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.12.2+tvOS 7.1+visionOS 1.0+watchOS 5.0+

``` source
class MPSeekCommandEvent
```

## Topics

### Changing the current seek behavior

var type: MPSeekCommandEventType

The type of seek command event.

### Constants

enum MPSeekCommandEventType

Defines the beginning and ending of seek events.

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

class MPSkipIntervalCommand

An object that defines the skip intervals for the player.

class MPSkipIntervalCommandEvent

An event requesting a change in the current skip interval.

