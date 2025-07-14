

- RealityKit
- SpatialAudioComponent
-  gain 

Instance Property

# gain

The overall level for all sounds that an entity emits.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
var gain: Audio.Decibel
```

## Discussion

The gain level is in relative decibels, in the range `[-Decibel.infinity, Decibel.zero]`, where `Decibel.zero` is the default.

