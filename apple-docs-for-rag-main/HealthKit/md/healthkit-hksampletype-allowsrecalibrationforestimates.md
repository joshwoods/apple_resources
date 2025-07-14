

- HealthKit
- HKSampleType
-  allowsRecalibrationForEstimates 

Instance Property

# allowsRecalibrationForEstimates

A Boolean value that indicates whether HealthKit supports recalibrating the prediction algorithm used to produce estimates for this sample type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 13.0+visionOS 1.0+watchOS 8.0+

``` source
var allowsRecalibrationForEstimates: Bool { get }
```

## Discussion

To recalibrate the data for this sample type, call the HKHealthStore class’s recalibrateEstimates(sampleType:date:completion:) method.

