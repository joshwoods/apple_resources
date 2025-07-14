

- RealityKit
- Audio
- Audio.DistanceAttenuation
-  Audio.DistanceAttenuation.rolloff(factor:) 

Case

# Audio.DistanceAttenuation.rolloff(factor:)

A standard geometric model for attenuating audio intensity naturally with distance, using a specified loss strength factor.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
case rolloff(factor: Double)
```

## Parameters 

`factor`  

The attenuation model’s loss strength factor in the range of `[0, Double.infinity]`.

## Discussion

The case’s default value is `1.0`, which attenuates spatial audio as the listener moves away from the source, similar to real-world physics. You can increase or decrease this effect by changing `factor` to other values. For example:

- `0.5` reduces the effect by 50%

- `2.0` doubles the effect

- `0.0` completely disables attenuation

