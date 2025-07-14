

- HealthKit
- HKElectrocardiogram
- HKElectrocardiogram.Classification
-  HKElectrocardiogram.Classification.unrecognized 

Case

# HKElectrocardiogram.Classification.unrecognized

A sample classification that this version of HealthKit doesn’t recognize.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
case unrecognized
```

## Discussion

For example, if the Apple Watch recording the sample is running a newer version of watchOS, it may support classification types that aren’t included in this version. You can check the version of the algorithm used to classify the ECG by reading the value of the sample’s HKMetadataKeyAppleECGAlgorithmVersion metadata key.

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

case inconclusivePoorReading

An unclassifiable sample caused by an unclear signal.

case inconclusiveOther

An unclassifiable sample caused by an unknown issue.

case notSet

A sample that doesn’t have an assigned classification.

