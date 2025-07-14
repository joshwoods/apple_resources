

- AVFoundation
- AVAssetReaderTrackOutput
-  audioTimePitchAlgorithm 

Instance Property

# audioTimePitchAlgorithm

The processing algorithm to use for scaled audio edits.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var audioTimePitchAlgorithm: AVAudioTimePitchAlgorithm { get set }
```

## Discussion

See Time Pitch Algorithm Settings for possible values. The system throws an exception if you set this property to a value other than one of the defined constants.

