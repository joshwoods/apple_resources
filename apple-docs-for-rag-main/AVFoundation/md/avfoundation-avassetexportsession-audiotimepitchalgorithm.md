

- AVFoundation
- AVAssetExportSession
-  audioTimePitchAlgorithm 

Instance Property

# audioTimePitchAlgorithm

A processing algorithm for managing audio pitch for scaled audio edits.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var audioTimePitchAlgorithm: AVAudioTimePitchAlgorithm { get set }
```

## Discussion

The default value is spectral.

## See Also

### Configuring Audio Output

var audioMix: AVAudioMix?

The parameters for audio mixing and an indication of whether to enable nondefault audio mixing for export.

