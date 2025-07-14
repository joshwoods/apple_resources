

- AppKit
- NSSound
-  volume 

Instance Property

# volume

The volume of the sound.

macOS 10.5+

``` source
var volume: Float { get set }
```

## Discussion

The valid range is between `0.0` and `1.0`.

The value of this property does not affect the systemwide volume.

## See Also

### Configuring Sounds

var name: NSSound.Name?

The name assigned to the sound.

typealias Name

func setName(NSSound.Name?) -> Bool

var currentTime: TimeInterval

The sound’s playback progress, in seconds.

var loops: Bool

A Boolean that indicates whether the sound restarts playback when it reaches the end of its content.

var playbackDeviceIdentifier: NSSound.PlaybackDeviceIdentifier?

Identifies the sound’s output device

typealias PlaybackDeviceIdentifier

