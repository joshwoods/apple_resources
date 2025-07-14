

- AppKit
- NSSound
-  name 

Instance Property

# name

The name assigned to the sound.

macOS

``` source
var name: NSSound.Name? { get }
```

## Discussion

The value of this property is `nil` when no name has been assigned.

## See Also

### Configuring Sounds

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

typealias PlaybackDeviceIdentifier

