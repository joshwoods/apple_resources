

- Media Player
- MPRemoteCommandCenter
-  seekForwardCommand 

Instance Property

# seekForwardCommand

The command object for seeking forward through a single media item.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.12.2+tvOS 7.1+visionOS 1.0+watchOS 5.0+

``` source
var seekForwardCommand: MPRemoteCommand { get }
```

## Discussion

Use the object in this property to register your app’s handler for seeking forward in the current track. In your handler, begin seeking forward through the current media item. You can disable the command if your app does not support it.

## See Also

### Navigating a track’s contents

var changePlaybackRateCommand: MPChangePlaybackRateCommand

The command object for changing the playback rate of the current media item.

var seekBackwardCommand: MPRemoteCommand

The command object for seeking backward through a single media item.

var skipBackwardCommand: MPSkipIntervalCommand

The command object for playing a previous point in a media item.

var skipForwardCommand: MPSkipIntervalCommand

The command object for playing a future point in a media item.

var changePlaybackPositionCommand: MPChangePlaybackPositionCommand

The command object for changing the playback position in a media item.

