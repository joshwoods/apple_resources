

- HealthKit
- HKElectrocardiogram
- HKElectrocardiogram.SymptomsStatus
-  HKElectrocardiogram.SymptomsStatus.present 

Case

# HKElectrocardiogram.SymptomsStatus.present

The user added a symptom when they recorded the ECG.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
case present
```

## Discussion

To access the symptoms, query for the HKCategorySample samples associated with the electrocardiogram sample.

## See Also

### Status

case none

The user didn’t enter a symptom when they recorded the ECG.

case notSet

