

- Media Player
-  MPRemoteCommandEvent 

Class

# MPRemoteCommandEvent

A description of a command sent by an external media player.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.12.2+tvOS 7.1+visionOS 1.0+watchOS 5.0+

``` source
class MPRemoteCommandEvent
```

## Topics

### Retrieving command information

var command: MPRemoteCommand

The command that sent the event.

var timestamp: TimeInterval

The time the event occurred.

## Relationships

### Inherits From

- NSObject

### Inherited By

- MPChangeLanguageOptionCommandEvent
- MPChangePlaybackPositionCommandEvent
- MPChangePlaybackRateCommandEvent
- MPChangeRepeatModeCommandEvent
- MPChangeShuffleModeCommandEvent
- MPFeedbackCommandEvent
- MPRatingCommandEvent
- MPSeekCommandEvent
- MPSkipIntervalCommandEvent

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Setting up the remote event handler

Becoming a now playable app

Ensure your app is eligible to become the Now Playing app by adopting best practices for providing Now Playing info and registering for remote command center actions.

class MPRemoteCommandCenter

An object that responds to remote control events sent by external accessories and system controls.

class MPRemoteCommand

An object that responds to remote command events.

