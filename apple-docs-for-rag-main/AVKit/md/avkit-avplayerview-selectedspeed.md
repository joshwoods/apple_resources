

- AVKit
- AVPlayerView
-  selectedSpeed 

Instance Property

# selectedSpeed

The currently selected playback speed.

macOS 13.0+

``` source
@MainActor
var selectedSpeed: AVPlaybackSpeed? { get }
```

## Discussion

This value reflects the associated player’s defaultRate property value. If you set the defaultRate to a value that doesn’t match a speed contained in the speeds property, the system sets this value to `nil`.

## See Also

### Configuring the Playback Speed

var speeds: [AVPlaybackSpeed]

A list of user-selectable playback speeds to show in the playback speed control.

func selectSpeed(AVPlaybackSpeed)

Selects a specified playback speed.

class AVPlaybackSpeed

An object that represents a user-selectable playback speed in a playback user interface.

