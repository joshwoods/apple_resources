

- HealthKit
-  HKAppleSleepingBreathingDisturbancesClassification 

Enumeration

# HKAppleSleepingBreathingDisturbancesClassification

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+watchOS 11.0+

``` source
enum HKAppleSleepingBreathingDisturbancesClassification
```

## Topics

### Enumeration Cases

case elevated

case notElevated

### Instance Properties

var minimum: HKQuantity

### Initializers

init?(classifying: HKQuantity)

init?(rawValue: Int)

### Default Implementations

CaseIterable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- CaseIterable
- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Mindfulness and sleep

static let mindfulSession: HKCategoryTypeIdentifier

A category sample type for recording a mindful session.

static let sleepAnalysis: HKCategoryTypeIdentifier

A category sample type for sleep analysis information.

static let appleSleepingWristTemperature: HKQuantityTypeIdentifier

A quantity sample type that records the wrist temperature during sleep.

