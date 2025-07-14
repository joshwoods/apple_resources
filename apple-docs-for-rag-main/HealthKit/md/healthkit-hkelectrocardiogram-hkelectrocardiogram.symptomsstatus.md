

- HealthKit
- HKElectrocardiogram
-  HKElectrocardiogram.SymptomsStatus 

Enumeration

# HKElectrocardiogram.SymptomsStatus

Values indicating whether the user entered a symptom when they recorded the ECG.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
enum SymptomsStatus
```

## Topics

### Status

case none

The user didn’t enter a symptom when they recorded the ECG.

case present

The user added a symptom when they recorded the ECG.

case notSet

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

### Accessing Overview Information

var classification: HKElectrocardiogram.Classification

The ECG’s classification.

enum Classification

Classifications returned by Apple Watch’s ECG algorithm.

var averageHeartRate: HKQuantity?

The user’s average heart rate during the ECG.

var symptomsStatus: HKElectrocardiogram.SymptomsStatus

A value that indicates whether the user entered a symptom when they recorded the ECG.

