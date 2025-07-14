

- Media Player
- MPRemoteCommandCenter
-  skipForwardCommand 

Instance Property

# skipForwardCommand

The command object for playing a future point in a media item.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.12.2+tvOS 7.1+visionOS 1.0+watchOS 5.0+

``` source
var skipForwardCommand: MPSkipIntervalCommand { get }
```

## Discussion

Use the object in this property to register your app’s handler for jumping to a future point in the current track. In your handler, skip forward by the amount specified in the event’s interval property. You can disable the command if your app does not support it.

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

var changePlaybackPositionCommand: MPChangePlaybackPositionCommand

The command object for changing the playback position in a media item.

