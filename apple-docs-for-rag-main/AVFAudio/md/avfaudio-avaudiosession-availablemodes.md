

- AVFAudio
- AVAudioSession
-  availableModes 

Instance Property

# availableModes

The audio session modes available on the device.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var availableModes: [AVAudioSession.Mode] { get }
```

## Discussion

Not every device supports every audio session mode. For example, the videoRecording mode isn’t available on a device that doesn’t support video recording.

Query this property to determine if the mode you’d like to use is available on the current device.

## See Also

### Inspecting mode configuration

var mode: AVAudioSession.Mode

The current audio session’s mode.

struct Mode

Audio session mode identifiers.

