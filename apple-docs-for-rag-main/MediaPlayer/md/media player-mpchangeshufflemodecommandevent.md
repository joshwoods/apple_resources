

- Media Player
-  MPChangeShuffleModeCommandEvent 

Class

# MPChangeShuffleModeCommandEvent

An event requesting a change in the shuffle mode.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.12.2+tvOS 8.0+visionOS 1.0+watchOS 5.0+

``` source
class MPChangeShuffleModeCommandEvent
```

## Topics

### Changing the shuffle mode

var shuffleType: MPShuffleType

The shuffle type used when fulfilling the event request.

var preservesShuffleMode: Bool

A Boolean value that indicates whether the shuffle mode is preserved between playback sessions.

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

class MPChangePlaybackRateCommandEvent

An event requesting a change in the playback rate.

class MPChangeLanguageOptionCommandEvent

An event requesting a change in the language option.

class MPChangeRepeatModeCommand

An object that responds to requests to change the current repeat mode used during playback.

class MPChangeRepeatModeCommandEvent

An event requesting a change in the repeat mode.

class MPChangeShuffleModeCommand

An object that responds to requests to change the current shuffle mode used during playback.

enum MPRepeatType

Indicates which items to play repeatedly.

enum MPShuffleType

Indicates which item types to shuffle.

