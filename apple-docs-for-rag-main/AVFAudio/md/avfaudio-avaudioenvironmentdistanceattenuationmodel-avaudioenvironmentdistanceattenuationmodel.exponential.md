

- AVFAudio
- AVAudioEnvironmentDistanceAttenuationModel
-  AVAudioEnvironmentDistanceAttenuationModel.exponential 

Case

# AVAudioEnvironmentDistanceAttenuationModel.exponential

An exponential model that describes the drop-off in gain as the source moves away from the listener.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
case exponential
```

## Discussion

The framework calculates this value as `distanceGain = (distance / referenceDistance) ^ (-rolloffFactor)`.

## See Also

### Attenuation Models

case inverse

An inverse model that describes the drop-off in gain as the source moves away from the listener.

case linear

A linear model that describes the drop-off in gain as the source moves away from the listener.

