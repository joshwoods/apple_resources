

- Speech
- SFVoiceAnalytics
-  shimmer 

Instance Property

# shimmer

The variation in vocal volume stability (amplitude) in each frame of a transcription segment, expressed in decibels.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+

``` source
@NSCopying
var shimmer: SFAcousticFeature { get }
```

## See Also

### Analyzing voice

class SFAcousticFeature

The value of a voice analysis metric.

var voicing: SFAcousticFeature

The likelihood of a voice in each frame of a transcription segment.

var pitch: SFAcousticFeature

The highness or lowness of the tone (fundamental frequency) in each frame of a transcription segment, expressed as a logarithm.

var jitter: SFAcousticFeature

The variation in pitch in each frame of a transcription segment, expressed as a percentage of the frame’s fundamental frequency.

