

- Media Player
-  MPChangePlaybackRateCommandEvent 

Class

# MPChangePlaybackRateCommandEvent

An event requesting a change in the playback rate.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.12.2+tvOS 7.1+visionOS 1.0+watchOS 5.0+

``` source
class MPChangePlaybackRateCommandEvent
```

## Topics

### Retrieving the playback rate

var playbackRate: Float

The chosen playback rate for the command event.

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

### Responding to changes to media playback mode events

class MPChangePlaybackRateCommand

An object that responds to requests to change the playback rate of the playing item.

class MPChangeLanguageOptionCommandEvent

An event requesting a change in the language option.

class MPChangeRepeatModeCommand

An object that responds to requests to change the current repeat mode used during playback.

class MPChangeRepeatModeCommandEvent

An event requesting a change in the repeat mode.

class MPChangeShuffleModeCommand

An object that responds to requests to change the current shuffle mode used during playback.

class MPChangeShuffleModeCommandEvent

An event requesting a change in the shuffle mode.

enum MPRepeatType

Indicates which items to play repeatedly.

enum MPShuffleType

Indicates which item types to shuffle.

