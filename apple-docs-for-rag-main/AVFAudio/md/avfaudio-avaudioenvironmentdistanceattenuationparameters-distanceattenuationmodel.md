

- AVFAudio
- AVAudioEnvironmentDistanceAttenuationParameters
-  distanceAttenuationModel 

Instance Property

# distanceAttenuationModel

The distance attenuation model that describes the drop-off in gain as the source moves away from the listener.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var distanceAttenuationModel: AVAudioEnvironmentDistanceAttenuationModel { get set }
```

## Discussion

The default value is the AVAudioEnvironmentDistanceAttenuationModel.inverse attenuation model.

## See Also

### Getting and Setting the Attenuation Model

enum AVAudioEnvironmentDistanceAttenuationModel

Types of distance attenuation models.

