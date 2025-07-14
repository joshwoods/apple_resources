

- Media Player
- MPRemoteCommandCenter
-  nextTrackCommand 

Instance Property

# nextTrackCommand

The command object for selecting the next track.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.12.2+tvOS 7.1+visionOS 1.0+watchOS 5.0+

``` source
var nextTrackCommand: MPRemoteCommand { get }
```

## Discussion

Use the object in this property to register your app’s handler for selecting the next track. In your handler, select the media item that follows the current media item. You can disable the command if your app does not support it.

## See Also

### Navigating between tracks

var previousTrackCommand: MPRemoteCommand

The command object for selecting the previous track.

var changeRepeatModeCommand: MPChangeRepeatModeCommand

The command object for changing the repeat mode.

var changeShuffleModeCommand: MPChangeShuffleModeCommand

The command object for changing the shuffle mode.

