

- Media Player
-  MPChangeLanguageOptionCommandEvent 

Class

# MPChangeLanguageOptionCommandEvent

An event requesting a change in the language option.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.12.2+tvOS 9.0+visionOS 1.0+watchOS 5.0+

``` source
class MPChangeLanguageOptionCommandEvent
```

## Topics

### Changing the language option

var languageOption: MPNowPlayingInfoLanguageOption

The requested language option to change.

var setting: MPChangeLanguageOptionSetting

The extent of the language setting change.

enum MPChangeLanguageOptionSetting

The states that determine when language option changes take effect.

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

