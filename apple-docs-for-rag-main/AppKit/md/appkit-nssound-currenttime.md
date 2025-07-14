

- AppKit
- NSSound
-  currentTime 

Instance Property

# currentTime

The sound’s playback progress, in seconds.

macOS 10.5+

``` source
var currentTime: TimeInterval { get set }
```

## Discussion

Sounds start with `currentTime == 0` and end with `currentTime == ([ duration] - 1)`.

This property is not archived, copied, or stored on the pasteboard.

## See Also

### Related Documentation

var duration: TimeInterval

The duration of the sound, in seconds.

### Configuring Sounds

var name: NSSound.Name?

The name assigned to the sound.

typealias Name

func setName(NSSound.Name?) -> Bool

var volume: Float

The volume of the sound.

var loops: Bool

A Boolean that indicates whether the sound restarts playback when it reaches the end of its content.

var playbackDeviceIdentifier: NSSound.PlaybackDeviceIdentifier?

Identifies the sound’s output device

typealias PlaybackDeviceIdentifier

