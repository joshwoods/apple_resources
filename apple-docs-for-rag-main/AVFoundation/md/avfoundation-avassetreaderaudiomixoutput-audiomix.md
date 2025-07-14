

- AVFoundation
- AVAssetReaderAudioMixOutput
-  audioMix 

Instance Property

# audioMix

The audio mix to use with this output.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
@NSCopying
var audioMix: AVAudioMix? { get set }
```

## Discussion

Use an audio mix to specify how an audio track’s volume changes over the media’s timeline.

## See Also

### Configuring Audio Settings

var audioTimePitchAlgorithm: AVAudioTimePitchAlgorithm

The processing algorithm to use for scaled audio edits.

