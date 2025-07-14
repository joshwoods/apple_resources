

- SensorKit
-  SRSpeechExpression 

Class

# SRSpeechExpression

An object that represents the metrics and voice analytics for a range of speech.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
class SRSpeechExpression
```

## Overview

Use the properties of this class to get the characteristics of the speech, such as the user’s confidence level and mood.

## Topics

### Getting speech metrics

var timeRange: CMTimeRange

The time range in the audio stream that the metrics and analytics apply to.

var version: String

The version of the algorithm that the system uses to generate the metrics and analytics.

### Getting speech analytics

var confidence: Double

The level of confidence of the speaker.

var mood: Double

An indication of how slurry, tired, or exhausted the speaker sounds compared to normal speech.

var valence: Double

The degree of positive or negative emotion or sentiment of the speaker.

var activation: Double

The level of energy or activation of the speaker.

var dominance: Double

The degree of how strong or meek the speaker sounds.

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
- Sendable

## See Also

### Analyzing speech

class SRSpeechMetrics

An object that represents metrics about a range of speech.

