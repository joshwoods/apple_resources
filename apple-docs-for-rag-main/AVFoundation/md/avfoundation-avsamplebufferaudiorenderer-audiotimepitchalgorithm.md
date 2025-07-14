

- AVFoundation
- AVSampleBufferAudioRenderer
-  audioTimePitchAlgorithm 

Instance Property

# audioTimePitchAlgorithm

The processing algorithm used to manage audio pitch at different rates.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var audioTimePitchAlgorithm: AVAudioTimePitchAlgorithm { get set }
```

## Discussion

The default value on iOS is lowQualityZeroLatency; on macOS, the default is timeDomain. The device automatically mutes audio when timebase is not supported by AVAudioTimePitchAlgorithm. Modifying this property while timebase is not `0.0` may cause the rate to briefly change to `0.0`.

## See Also

### Configuring Time and Pitch

struct AVAudioTimePitchAlgorithm

An algorithm used to set the audio pitch as the rate changes.

