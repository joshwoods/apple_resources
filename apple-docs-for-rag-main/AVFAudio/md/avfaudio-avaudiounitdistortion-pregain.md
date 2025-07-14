

- AVFAudio
- AVAudioUnitDistortion
-  preGain 

Instance Property

# preGain

The gain that the audio unit applies to the signal before distortion, in decibels.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var preGain: Float { get set }
```

## Discussion

The default value is `-6 dB`. The valid range of values is `-80 dB` to `20 dB`.

## See Also

### Getting and setting the distortion values

var wetDryMix: Float

The blend of the distorted and dry signals.

