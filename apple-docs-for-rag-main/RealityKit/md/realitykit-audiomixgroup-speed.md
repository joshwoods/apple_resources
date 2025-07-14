

- RealityKit
- AudioMixGroup
-  speed 

Instance Property

# speed

The rate of playback for an audio mix group.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
var speed: Double
```

## Discussion

The system limits the rate of playback to the range of `[0.25, 4]`. The default speed is `1`, which is equivalent to a normal playback rate.

Note

AudioGeneratorController ignores this value.

