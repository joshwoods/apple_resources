

- Media Player
- MPRemoteCommandCenter
-  changePlaybackPositionCommand 

Instance Property

# changePlaybackPositionCommand

The command object for changing the playback position in a media item.

iOS 9.1+iPadOS 9.1+Mac Catalyst 13.1+macOS 10.12.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var changePlaybackPositionCommand: MPChangePlaybackPositionCommand { get }
```

## Discussion

Use the object in this property to register your app’s handler for changing the playback position for the playlist. In your handler, change the playback position to the new value. You can disable the command if your app does not support it.

## See Also

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

