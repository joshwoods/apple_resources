

- HealthKit
-  HKHeartRateMotionContext 

Enumeration

# HKHeartRateMotionContext

Values that indicate the user’s level of activity when the heart rate sample was measured.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 4.0+

``` source
enum HKHeartRateMotionContext
```

## Topics

### Motion Contextes

case active

A value indicating that the user was in motion during the heart rate sample.

case notSet

A value indicating that the user’s activity level could not be determined.

case sedentary

A value indicating that the user has been still for at least 5 minutes prior to the heart rate sample.

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

### Related Documentation

static let heartRate: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s heart rate.

