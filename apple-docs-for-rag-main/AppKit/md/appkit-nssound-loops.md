

- AppKit
- NSSound
-  loops 

Instance Property

# loops

A Boolean that indicates whether the sound restarts playback when it reaches the end of its content.

macOS 10.5+

``` source
var loops: Bool { get set }
```

## Discussion

When the value of this property is true, the sounds restarts playback when it finishes and does not send sound(_:didFinishPlaying:) to its delegate when it reaches the end of its content and restarts playback. The default value of this property is false.

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

var playbackDeviceIdentifier: NSSound.PlaybackDeviceIdentifier?

Identifies the sound’s output device

typealias PlaybackDeviceIdentifier

