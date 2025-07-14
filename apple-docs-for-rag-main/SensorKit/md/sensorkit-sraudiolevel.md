

- SensorKit
-  SRAudioLevel 

Class

# SRAudioLevel

An object that represents the audio level for a range of speech.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
class SRAudioLevel
```

## Overview

Use the loudness property to get the value of the audio level.

## Topics

### Getting metrics

var timeRange: CMTimeRange

The time range in the audio stream that the level applies to.

var loudness: Double

The measure of the audio level in decibels.

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

### Getting speech metrics and analytics

var audioLevel: SRAudioLevel?

The audio level of the speech.

var speechRecognition: SFSpeechRecognitionResult?

The partial or final results of the speech recognition request.

var soundClassification: SNClassificationResult?

The highest-ranking classifications in the time range.

var speechExpression: SRSpeechExpression?

The metrics and voice analytics for the range of speech.

