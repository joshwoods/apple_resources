

- HealthKit
-  HKHeartRateRecoveryTestType 

Enumeration

# HKHeartRateRecoveryTestType

The test that measured a person’s heart-rate recovery.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
enum HKHeartRateRecoveryTestType
```

## Topics

### Heart-rate recovery tests

case maxExercise

Measures a person’s actual heart-rate recovery.

case predictionNonExercise

A test that estimates a person’s heart-rate recovery without using exercise.

case predictionSubMaxExercise

A test that estimates a person’s heart-rate recovery using lower-intensity exercise.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

