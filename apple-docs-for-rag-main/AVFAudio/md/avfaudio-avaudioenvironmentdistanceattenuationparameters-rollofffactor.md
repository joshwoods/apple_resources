

- AVFAudio
- AVAudioEnvironmentDistanceAttenuationParameters
-  rolloffFactor 

Instance Property

# rolloffFactor

A factor that determines the attenuation curve.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var rolloffFactor: Float { get set }
```

## Discussion

A higher value results in a steeper attenuation curve. The default value is `1.0`, and the value must be greater than `0.0`.

This property is relevant for AVAudioEnvironmentDistanceAttenuationModel.exponential, AVAudioEnvironmentDistanceAttenuationModel.inverse, and AVAudioEnvironmentDistanceAttenuationModel.linear.

## See Also

### Getting and Setting the Attenuation Values

var maximumDistance: Float

The distance beyond which the node applies no further attenuation, in meters.

var referenceDistance: Float

The minimum distance at which the node applies attenuation, in meters.

