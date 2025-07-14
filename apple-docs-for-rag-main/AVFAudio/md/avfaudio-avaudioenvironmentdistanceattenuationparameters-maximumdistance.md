

- AVFAudio
- AVAudioEnvironmentDistanceAttenuationParameters
-  maximumDistance 

Instance Property

# maximumDistance

The distance beyond which the node applies no further attenuation, in meters.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var maximumDistance: Float { get set }
```

## Discussion

The default value is `100000.0` meters.

This property is relevant for AVAudioEnvironmentDistanceAttenuationModel.inverse.

## See Also

### Getting and Setting the Attenuation Values

var referenceDistance: Float

The minimum distance at which the node applies attenuation, in meters.

var rolloffFactor: Float

A factor that determines the attenuation curve.

