

- AppKit
- NSSound
-  NSSound.PlaybackDeviceIdentifier 

Type Alias

# NSSound.PlaybackDeviceIdentifier

macOS

``` source
typealias PlaybackDeviceIdentifier = String
```

## See Also

### Configuring Sounds

var name: NSSound.Name?

The name assigned to the sound.

typealias Name

func setName(NSSound.Name?) -> Bool

var volume: Float

The volume of the sound.

var currentTime: TimeInterval

The sound’s playback progress, in seconds.

var loops: Bool

A Boolean that indicates whether the sound restarts playback when it reaches the end of its content.

var playbackDeviceIdentifier: NSSound.PlaybackDeviceIdentifier?

Identifies the sound’s output device

