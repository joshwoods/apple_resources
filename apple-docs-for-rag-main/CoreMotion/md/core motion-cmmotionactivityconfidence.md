

- Core Motion
-  CMMotionActivityConfidence 

Enumeration

# CMMotionActivityConfidence

The confidence that the motion data is accurate.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 2.0+

``` source
enum CMMotionActivityConfidence
```

## Topics

### Constants

case low

Confidence is low.

case medium

Confidence is good.

case high

Confidence is high.

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

### Getting Metadata for the Motion

var startDate: Date

The time at which the change in motion occurred.

var confidence: CMMotionActivityConfidence

The confidence in the assessment of the motion type.

