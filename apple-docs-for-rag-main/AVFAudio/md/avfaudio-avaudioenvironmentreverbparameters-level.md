

- AVFAudio
- AVAudioEnvironmentReverbParameters
-  level 

Instance Property

# level

Controls the amount of reverb, in decibels.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var level: Float { get set }
```

## Discussion

The default value is `0.0`. The values must be within the range of `-40` to `40` dB.

## See Also

### Getting and Setting Reverb Values

var filterParameters: AVAudioUnitEQFilterParameters

A filter that the system applies to the output.

func loadFactoryReverbPreset(AVAudioUnitReverbPreset)

Loads one of the reverbs factory presets.

