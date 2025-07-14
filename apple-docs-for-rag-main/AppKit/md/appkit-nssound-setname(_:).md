

- AppKit
- NSSound
-  setName(\_:) 

Instance Method

# setName(\_:)

macOS

``` source
func setName(_ string: NSSound.Name?) -> Bool
```

## See Also

### Configuring Sounds

var name: NSSound.Name?

The name assigned to the sound.

typealias Name

var volume: Float

The volume of the sound.

var currentTime: TimeInterval

The sound’s playback progress, in seconds.

var loops: Bool

A Boolean that indicates whether the sound restarts playback when it reaches the end of its content.

var playbackDeviceIdentifier: NSSound.PlaybackDeviceIdentifier?

Identifies the sound’s output device

typealias PlaybackDeviceIdentifier

