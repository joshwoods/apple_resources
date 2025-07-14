

- RealityKit
- Audio
- Audio.DistanceAttenuation
-  default 

Type Property

# default

The default distance attenuation, which uses a rolloff model that mimics real-world physics.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
static let `default`: Audio.DistanceAttenuation
```

## Discussion

The Audio.DistanceAttenuation.rolloff(factor:) model attenuates spatial audio with a factor of `1.0` as the listener moves away from the source.

