

- SensorKit
-  SRSpeechMetrics 

Class

# SRSpeechMetrics

An object that represents metrics about a range of speech.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
class SRSpeechMetrics
```

## Overview

To get the audio level, use the audioLevel property. Otherwise, use the speechRecognition, soundClassification, and speechExpression properties to get characteristics of the speech.

The siriSpeechMetrics sensor provides this class as its sample type.

## Topics

### Getting session information

var sessionIdentifier: String

An identifier for the audio session.

var sessionFlags: SRSpeechMetrics.SessionFlags

Details about the audio processing.

struct SessionFlags

Possible details about processing an audio stream.

var timeSinceAudioStart: TimeInterval

The number of seconds since the start of the audio stream.

var timestamp: Date

The date and time when the speech occurs.

### Getting speech metrics and analytics

var audioLevel: SRAudioLevel?

The audio level of the speech.

class SRAudioLevel

An object that represents the audio level for a range of speech.

var speechRecognition: SFSpeechRecognitionResult?

The partial or final results of the speech recognition request.

var soundClassification: SNClassificationResult?

The highest-ranking classifications in the time range.

var speechExpression: SRSpeechExpression?

The metrics and voice analytics for the range of speech.

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

class SRSpeechExpression

An object that represents the metrics and voice analytics for a range of speech.

