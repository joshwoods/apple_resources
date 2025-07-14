

- Media Player
-  MPRemoteCommandCenter 

Class

# MPRemoteCommandCenter

An object that responds to remote control events sent by external accessories and system controls.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.12.2+tvOS 7.1+visionOS 1.0+watchOS 5.0+

``` source
class MPRemoteCommandCenter
```

## Mentioned in 

Handling external player events notifications

## Overview

Don’t create instances of this class yourself. Instead, use the shared() method to retrieve the shared command center object. The properties of the shared command center object contain MPRemoteCommand objects that respond to the various kinds of remote control events. You configure these objects to respond to the events you’re interested to handle in your app.

## Topics

### Retrieving the shared instance

class func shared() -> MPRemoteCommandCenter

Returns the shared object you use to access the system’s remote command objects.

### Playback commands

var pauseCommand: MPRemoteCommand

The command object for pausing playback of the current item.

var playCommand: MPRemoteCommand

The command object for starting playback of the current item.

var stopCommand: MPRemoteCommand

The command object for stopping playback of the current item.

var togglePlayPauseCommand: MPRemoteCommand

The command object for toggling between playing and pausing the current item.

### Navigating between tracks

var nextTrackCommand: MPRemoteCommand

The command object for selecting the next track.

var previousTrackCommand: MPRemoteCommand

The command object for selecting the previous track.

var changeRepeatModeCommand: MPChangeRepeatModeCommand

The command object for changing the repeat mode.

var changeShuffleModeCommand: MPChangeShuffleModeCommand

The command object for changing the shuffle mode.

### Navigating a track’s contents

var changePlaybackRateCommand: MPChangePlaybackRateCommand

The command object for changing the playback rate of the current media item.

var seekBackwardCommand: MPRemoteCommand

The command object for seeking backward through a single media item.

var seekForwardCommand: MPRemoteCommand

The command object for seeking forward through a single media item.

var skipBackwardCommand: MPSkipIntervalCommand

The command object for playing a previous point in a media item.

var skipForwardCommand: MPSkipIntervalCommand

The command object for playing a future point in a media item.

var changePlaybackPositionCommand: MPChangePlaybackPositionCommand

The command object for changing the playback position in a media item.

### Rating a media item

var ratingCommand: MPRatingCommand

The command object for rating a media item.

var likeCommand: MPFeedbackCommand

The command object for indicating that a user likes what is currently playing.

var dislikeCommand: MPFeedbackCommand

The command object for indicating that a user dislikes what is currently playing.

### Bookmarking a media item

var bookmarkCommand: MPFeedbackCommand

The command object for indicating that a user wants to remember a media item.

### Enabling language options

var enableLanguageOptionCommand: MPRemoteCommand

The command object for enabling a language option.

var disableLanguageOptionCommand: MPRemoteCommand

The command object for disabling a language option

## Relationships

### Inherits From

- NSObject

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

class MPRemoteCommand

An object that responds to remote command events.

class MPRemoteCommandEvent

A description of a command sent by an external media player.

