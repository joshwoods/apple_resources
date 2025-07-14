

- AVFAudio
- AVAudioEnvironmentDistanceAttenuationParameters
-  referenceDistance 

Instance Property

# referenceDistance

The minimum distance at which the node applies attenuation, in meters.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var referenceDistance: Float { get set }
```

## Discussion

The default value is `1.0` meter.

This property is relevant for AVAudioEnvironmentDistanceAttenuationModel.inverse and AVAudioEnvironmentDistanceAttenuationModel.linear.

## See Also

### Getting and Setting the Attenuation Values

var maximumDistance: Float

The distance beyond which the node applies no further attenuation, in meters.

var rolloffFactor: Float

A factor that determines the attenuation curve.

