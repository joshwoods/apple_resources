

- RealityKit
- SpatialAudioComponent
-  directLevel 

Instance Property

# directLevel

The level of the direct unreverberated signal that an entity emits.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
var directLevel: Audio.Decibel
```

## Discussion

The direct level is in relative decibels, in the range `[-Decibel.infinity, Decibel.zero]`, where `Decibel.zero` is the default.

