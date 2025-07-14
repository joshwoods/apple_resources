

- HealthKit
- HKElectrocardiogram
-  HKElectrocardiogram.Classification 

Enumeration

# HKElectrocardiogram.Classification

Classifications returned by Apple Watch’s ECG algorithm.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
enum Classification
```

## Topics

### Classifications

case sinusRhythm

The sample exhibits no signs of atrial fibrillation.

case atrialFibrillation

The sample exhibits signs of atrial fibrillation.

case inconclusiveHighHeartRate

An unclassifiable sample caused by a rapid heart rate.

case inconclusiveLowHeartRate

An unclassifiable sample caused by a heart rate below 50 bpm.

case inconclusivePoorReading

An unclassifiable sample caused by an unclear signal.

case inconclusiveOther

An unclassifiable sample caused by an unknown issue.

case unrecognized

A sample classification that this version of HealthKit doesn’t recognize.

case notSet

A sample that doesn’t have an assigned classification.

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

var averageHeartRate: HKQuantity?

The user’s average heart rate during the ECG.

var symptomsStatus: HKElectrocardiogram.SymptomsStatus

A value that indicates whether the user entered a symptom when they recorded the ECG.

enum SymptomsStatus

Values indicating whether the user entered a symptom when they recorded the ECG.

