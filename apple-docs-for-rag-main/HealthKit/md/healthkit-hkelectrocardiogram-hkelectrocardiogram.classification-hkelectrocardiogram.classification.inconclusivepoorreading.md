

- HealthKit
- HKElectrocardiogram
- HKElectrocardiogram.Classification
-  HKElectrocardiogram.Classification.inconclusivePoorReading 

Case

# HKElectrocardiogram.Classification.inconclusivePoorReading

An unclassifiable sample caused by an unclear signal.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
case inconclusivePoorReading
```

## Discussion

Apple Watch reports a poor recording when circumstances cause the watch to collect insufficient or inaccurate data, such as when the user wears the watch too loosely on their wrist, or if the user’s arm isn’t resting on a firm surface. The user can make another attempt at measuring their ECG after fixing the issue.

## See Also

### Classifications

case sinusRhythm

The sample exhibits no signs of atrial fibrillation.

case atrialFibrillation

The sample exhibits signs of atrial fibrillation.

case inconclusiveHighHeartRate

An unclassifiable sample caused by a rapid heart rate.

case inconclusiveLowHeartRate

An unclassifiable sample caused by a heart rate below 50 bpm.

case inconclusiveOther

An unclassifiable sample caused by an unknown issue.

case unrecognized

A sample classification that this version of HealthKit doesn’t recognize.

case notSet

A sample that doesn’t have an assigned classification.

