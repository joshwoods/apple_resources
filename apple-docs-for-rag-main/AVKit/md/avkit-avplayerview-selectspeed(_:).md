

- AVKit
- AVPlayerView
-  selectSpeed(\_:) 

Instance Method

# selectSpeed(\_:)

Selects a specified playback speed.

macOS 13.0+

``` source
@MainActor
func selectSpeed(_ speed: AVPlaybackSpeed)
```

## Parameters 

`speed`  

The playback speed to select.

## Discussion

If you call this method with a speed that isn’t contained in the speeds property, the system ignores the call.

## See Also

### Configuring the Playback Speed

var speeds: [AVPlaybackSpeed]

A list of user-selectable playback speeds to show in the playback speed control.

var selectedSpeed: AVPlaybackSpeed?

The currently selected playback speed.

class AVPlaybackSpeed

An object that represents a user-selectable playback speed in a playback user interface.

