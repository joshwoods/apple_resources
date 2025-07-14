

- AVFoundation
- AVAudioMix
-  inputParameters 

Instance Property

# inputParameters

An array of input parameters for the mix.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var inputParameters: [AVAudioMixInputParameters] { get }
```

## Discussion

The array contains instances of AVAudioMixInputParameters.

Note

An instance of AVAudioMixInputParameters isn’t required for each audio track that contributes to the mix. Audio for those without associated `AVAudioMixInputParameters` objects are included in the mix and processed according to the default behavior.

