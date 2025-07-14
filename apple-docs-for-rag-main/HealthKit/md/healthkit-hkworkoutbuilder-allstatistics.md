

- HealthKit
- HKWorkoutBuilder
-  allStatistics 

Instance Property

# allStatistics

A dictionary that contains all the statistics for the workout builder.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
var allStatistics: [HKQuantityType : HKStatistics] { get }
```

## Discussion

HealthKit calculates an HKStatistics object for each HKQuantityType, based on the HKQuantitySample objects collected by the workout builder.

