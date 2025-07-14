

- Core Motion
-  CMHighFrequencyHeartRateDataConfidence 

Enumeration

# CMHighFrequencyHeartRateDataConfidence

The level of confidence in the accuracy of the heart rate data.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 1.0+watchOS 10.0+

``` source
enum CMHighFrequencyHeartRateDataConfidence
```

## Topics

### Levels of confidence

case low

A low level of confidence in the heart rate data.

case medium

A medium level of confidence in the heart rate data.

case high

A high level of confidence in the heart rate data.

case highest

The highest level of confidence in the heart rate data.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing heart rate data

var heartRate: Double

The heart rate value in units of beats per minute (BPM).

var confidence: CMHighFrequencyHeartRateDataConfidence

The confidence level of the heart rate value.

