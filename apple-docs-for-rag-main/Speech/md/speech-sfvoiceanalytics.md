

- Speech
-  SFVoiceAnalytics 

Class

# SFVoiceAnalytics

A collection of vocal analysis metrics.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+

``` source
class SFVoiceAnalytics
```

## Overview

Use an SFAcousticFeature object to access the `SFVoiceAnalytics` insights. Voice analytics include the following features:

- Use jitter to measure how pitch varies in audio.

- Use shimmer to measure how amplitude varies in audio.

- Use pitch to measure the highness and lowness of the tone.

- Use voicing to identify voiced regions in speech.

These results are part of the SFTranscriptionSegment object and are available when the system sends the isFinal flag.

## Topics

### Analyzing voice

class SFAcousticFeature

The value of a voice analysis metric.

var voicing: SFAcousticFeature

The likelihood of a voice in each frame of a transcription segment.

var pitch: SFAcousticFeature

The highness or lowness of the tone (fundamental frequency) in each frame of a transcription segment, expressed as a logarithm.

var jitter: SFAcousticFeature

The variation in pitch in each frame of a transcription segment, expressed as a percentage of the frame’s fundamental frequency.

var shimmer: SFAcousticFeature

The variation in vocal volume stability (amplitude) in each frame of a transcription segment, expressed in decibels.

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

