

- RealityKit
- AudioPlaybackController
-  gain 

Instance Property

# gain

The individual gain in decibels of the audio playback controller output.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
var gain: AudioPlaybackController.Decibel { get set }
```

## Discussion

Use the fade(to:duration:) method to change the gain gradually and create smooth transitions.

## See Also

### Setting the volume

func fade(to: AudioPlaybackController.Decibel, duration: TimeInterval)

Transitions the gain to the given value over a time interval using a linear curve.

