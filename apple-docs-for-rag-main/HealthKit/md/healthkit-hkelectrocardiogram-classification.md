

- HealthKit
- HKElectrocardiogram
-  classification 

Instance Property

# classification

The ECG’s classification.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
var classification: HKElectrocardiogram.Classification { get }
```

## See Also

### Accessing Overview Information

enum Classification

Classifications returned by Apple Watch’s ECG algorithm.

var averageHeartRate: HKQuantity?

The user’s average heart rate during the ECG.

var symptomsStatus: HKElectrocardiogram.SymptomsStatus

A value that indicates whether the user entered a symptom when they recorded the ECG.

enum SymptomsStatus

Values indicating whether the user entered a symptom when they recorded the ECG.

