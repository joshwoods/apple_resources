

- HealthKit
- HKElectrocardiogram
-  symptomsStatus 

Instance Property

# symptomsStatus

A value that indicates whether the user entered a symptom when they recorded the ECG.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
var symptomsStatus: HKElectrocardiogram.SymptomsStatus { get }
```

## Discussion

If the value is HKElectrocardiogram.SymptomsStatus.present, you can access the symptoms by querying for the HKCategorySample samples associated with the electrocardiogram sample. Use predicateForObjectsAssociated(electrocardiogram:) to create the predicate for the associated symptoms.

## See Also

### Accessing Overview Information

var classification: HKElectrocardiogram.Classification

The ECG’s classification.

enum Classification

Classifications returned by Apple Watch’s ECG algorithm.

var averageHeartRate: HKQuantity?

The user’s average heart rate during the ECG.

enum SymptomsStatus

Values indicating whether the user entered a symptom when they recorded the ECG.

