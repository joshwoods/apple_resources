

- AVFoundation
- AVAssetExportSession
-  audioMix 

Instance Property

# audioMix

The parameters for audio mixing and an indication of whether to enable nondefault audio mixing for export.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
@NSCopying
var audioMix: AVAudioMix? { get set }
```

## Discussion

This value is key-value observable.

## See Also

### Configuring Audio Output

var audioTimePitchAlgorithm: AVAudioTimePitchAlgorithm

A processing algorithm for managing audio pitch for scaled audio edits.

