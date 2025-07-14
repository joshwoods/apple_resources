

- Speech
- SFVoiceAnalytics
-  voicing 

Instance Property

# voicing

The likelihood of a voice in each frame of a transcription segment.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+

``` source
@NSCopying
var voicing: SFAcousticFeature { get }
```

## Discussion

The `voicing` value is expressed as a probability in the range `[0.0, 1.0]`.

## See Also

### Analyzing voice

class SFAcousticFeature

The value of a voice analysis metric.

var pitch: SFAcousticFeature

The highness or lowness of the tone (fundamental frequency) in each frame of a transcription segment, expressed as a logarithm.

var jitter: SFAcousticFeature

The variation in pitch in each frame of a transcription segment, expressed as a percentage of the frame’s fundamental frequency.

var shimmer: SFAcousticFeature

The variation in vocal volume stability (amplitude) in each frame of a transcription segment, expressed in decibels.

