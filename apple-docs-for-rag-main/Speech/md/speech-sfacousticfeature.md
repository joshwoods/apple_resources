

- Speech
-  SFAcousticFeature 

Class

# SFAcousticFeature

The value of a voice analysis metric.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+

``` source
class SFAcousticFeature
```

## Topics

### Inspecting a feature

var frameDuration: TimeInterval

The duration of the audio frame.

var acousticFeatureValuePerFrame: [Double]

An array of feature values, one value per audio frame, corresponding to a transcript segment of recorded audio.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Analyzing voice

var voicing: SFAcousticFeature

The likelihood of a voice in each frame of a transcription segment.

var pitch: SFAcousticFeature

The highness or lowness of the tone (fundamental frequency) in each frame of a transcription segment, expressed as a logarithm.

var jitter: SFAcousticFeature

The variation in pitch in each frame of a transcription segment, expressed as a percentage of the frame’s fundamental frequency.

var shimmer: SFAcousticFeature

The variation in vocal volume stability (amplitude) in each frame of a transcription segment, expressed in decibels.

