

- Media Player
-  MPChangePlaybackRateCommand 

Class

# MPChangePlaybackRateCommand

An object that responds to requests to change the playback rate of the playing item.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.12.2+tvOS 7.1+visionOS 1.0+watchOS 5.0+

``` source
class MPChangePlaybackRateCommand
```

## Overview

Apps can change the current playback rate of a media item to one of the supported rates defined by the supportedPlaybackRates property.

## Topics

### Retrieving playback rates

var supportedPlaybackRates: [NSNumber]

The supported playback rates for a media item.

## Relationships

### Inherits From

- MPRemoteCommand

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Responding to changes to media playback mode events

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

enum MPShuffleType

Indicates which item types to shuffle.

