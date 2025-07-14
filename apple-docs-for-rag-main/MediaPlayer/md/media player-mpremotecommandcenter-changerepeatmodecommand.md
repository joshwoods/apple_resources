

- Media Player
- MPRemoteCommandCenter
-  changeRepeatModeCommand 

Instance Property

# changeRepeatModeCommand

The command object for changing the repeat mode.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.12.2+tvOS 7.1+visionOS 1.0+watchOS 5.0+

``` source
var changeRepeatModeCommand: MPChangeRepeatModeCommand { get }
```

## Discussion

Use the object in this property to register your app’s handler for changing the repeat mode for the playlist. In your handler, change the repeat mode to the new value. You can disable the command if your app does not support it.

## See Also

### Navigating between tracks

var nextTrackCommand: MPRemoteCommand

The command object for selecting the next track.

var previousTrackCommand: MPRemoteCommand

The command object for selecting the previous track.

var changeShuffleModeCommand: MPChangeShuffleModeCommand

The command object for changing the shuffle mode.

