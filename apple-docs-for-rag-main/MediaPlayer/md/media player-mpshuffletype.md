

- Media Player
-  MPShuffleType 

Enumeration

# MPShuffleType

Indicates which item types to shuffle.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.12.2+tvOSvisionOS 1.0+watchOS 5.0+

``` source
enum MPShuffleType
```

## Topics

### Shuffle types

case off

Nothing is shuffled during playback.

case items

Individual items are shuffled during playback.

case collections

Collections of items are shuffled during playback.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

class MPChangeShuffleModeCommandEvent

An event requesting a change in the shuffle mode.

enum MPRepeatType

Indicates which items to play repeatedly.

