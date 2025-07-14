

- AVFAudio
- AVAudioUnitDistortion
-  wetDryMix 

Instance Property

# wetDryMix

The blend of the distorted and dry signals.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var wetDryMix: Float { get set }
```

## Discussion

You specify the blend as a percentage. The default value is `50%`. The valid range is `0%` through `100%`, where `0` represents all dry.

## See Also

### Getting and setting the distortion values

var preGain: Float

The gain that the audio unit applies to the signal before distortion, in decibels.

