

- Media Player
- MPRemoteCommandCenter
-  previousTrackCommand 

Instance Property

# previousTrackCommand

The command object for selecting the previous track.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.12.2+tvOS 7.1+visionOS 1.0+watchOS 5.0+

``` source
var previousTrackCommand: MPRemoteCommand { get }
```

## Discussion

Use the object in this property to register your app’s handler for selecting the previous track. In your handler, select the media item that precedes the current media item. You can disable the command if your app does not support it.

## See Also

### Navigating between tracks

var nextTrackCommand: MPRemoteCommand

The command object for selecting the next track.

var changeRepeatModeCommand: MPChangeRepeatModeCommand

The command object for changing the repeat mode.

var changeShuffleModeCommand: MPChangeShuffleModeCommand

The command object for changing the shuffle mode.

