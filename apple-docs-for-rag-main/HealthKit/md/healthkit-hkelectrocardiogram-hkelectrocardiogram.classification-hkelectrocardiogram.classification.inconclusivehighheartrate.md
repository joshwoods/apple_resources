

- HealthKit
- HKElectrocardiogram
- HKElectrocardiogram.Classification
-  HKElectrocardiogram.Classification.inconclusiveHighHeartRate 

Case

# HKElectrocardiogram.Classification.inconclusiveHighHeartRate

An unclassifiable sample caused by a rapid heart rate.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
case inconclusiveHighHeartRate
```

## Discussion

The HKAppleECGAlgorithmVersion.version1 algorithm can categorize heart rates below 120 BPM. HKAppleECGAlgorithmVersion.version2 can categorize heart rates up to 150 BPM.

## See Also

### Classifications

case sinusRhythm

The sample exhibits no signs of atrial fibrillation.

case atrialFibrillation

The sample exhibits signs of atrial fibrillation.

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

