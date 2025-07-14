

- AVFoundation
- AVMutableAudioMix
-  inputParameters 

Instance Property

# inputParameters

An array of input parameters for the mix.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var inputParameters: [AVAudioMixInputParameters] { get set }
```

## Discussion

The array contains instances of AVAudioMixInputParameters. You don’t need an instance for each audio track that contributes to the mix. By default, the system processes audio for those tracks without an associated `AVAudioMixInputParameters` instance.

Warning

Specifying multiple `AVAudioMixInputParameters` for the same track has undefined behavior. Use only one instance per track in an audio mix.

