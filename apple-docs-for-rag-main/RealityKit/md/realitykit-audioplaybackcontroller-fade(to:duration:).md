

- RealityKit
- AudioPlaybackController
-  fade(to:duration:) 

Instance Method

# fade(to:duration:)

Transitions the gain to the given value over a time interval using a linear curve.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func fade(
    to newValue: AudioPlaybackController.Decibel,
    duration: TimeInterval
)
```

## Parameters 

`newValue`  

The target decibel level.

`duration`  

How long in seconds the fade should last.

## See Also

### Setting the volume

var gain: AudioPlaybackController.Decibel

The individual gain in decibels of the audio playback controller output.

