

- Media Player
- MPRemoteCommandCenter
-  stopCommand 

Instance Property

# stopCommand

The command object for stopping playback of the current item.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.12.2+tvOS 7.1+visionOS 1.0+watchOS 5.0+

``` source
var stopCommand: MPRemoteCommand { get }
```

## Discussion

Use the object in this property to register your app’s handler for stopping playback of the current track. In your handler, stop playback the current item. You can disable the command if your app does not support it.

## See Also

### Playback commands

var pauseCommand: MPRemoteCommand

The command object for pausing playback of the current item.

var playCommand: MPRemoteCommand

The command object for starting playback of the current item.

var togglePlayPauseCommand: MPRemoteCommand

The command object for toggling between playing and pausing the current item.

