

- HealthKit
- HKElectrocardiogram
-  averageHeartRate 

Instance Property

# averageHeartRate

The user’s average heart rate during the ECG.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
@NSCopying
var averageHeartRate: HKQuantity? { get }
```

## See Also

### Accessing Overview Information

var classification: HKElectrocardiogram.Classification

The ECG’s classification.

enum Classification

Classifications returned by Apple Watch’s ECG algorithm.

var symptomsStatus: HKElectrocardiogram.SymptomsStatus

A value that indicates whether the user entered a symptom when they recorded the ECG.

enum SymptomsStatus

Values indicating whether the user entered a symptom when they recorded the ECG.

