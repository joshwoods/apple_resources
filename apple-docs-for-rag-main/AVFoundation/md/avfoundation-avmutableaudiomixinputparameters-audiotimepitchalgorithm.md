

- AVFoundation
- AVMutableAudioMixInputParameters
-  audioTimePitchAlgorithm 

Instance Property

# audioTimePitchAlgorithm

The processing algorithm used to manage audio pitch for scaled audio edits.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var audioTimePitchAlgorithm: AVAudioTimePitchAlgorithm? { get set }
```

## Discussion

The supported constants are defined in Time Pitch Algorithm Settings. An invalidArgumentException is raised if this property is set to a value other than the defined constants.

## See Also

### Time Pitch Settings

struct AVAudioTimePitchAlgorithm

An algorithm used to set the audio pitch as the rate changes.

