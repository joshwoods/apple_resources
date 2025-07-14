

- RealityKit
- AudioMixGroup
-  fade(to:duration:) 

Instance Method

# fade(to:duration:)

Transitions the gain to a value over a time interval using a linear curve.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
mutating func fade(
    to gain: Audio.Decibel,
    duration: TimeInterval
)
```

## Parameters 

`gain`  

The overall level for audio from a group after the fade is complete.

`duration`  

The duration of the fade in seconds.

