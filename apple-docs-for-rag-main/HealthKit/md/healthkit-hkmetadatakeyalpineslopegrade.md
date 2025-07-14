

- HealthKit
-  HKMetadataKeyAlpineSlopeGrade 

Global Variable

# HKMetadataKeyAlpineSlopeGrade

A key that indicates the percent slope of a ski run.

iOS 11.2+iPadOS 11.2+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 4.2+

``` source
let HKMetadataKeyAlpineSlopeGrade: String
```

## Mentioned in 

Receiving Downhill Skiing and Snowboarding Data

## Discussion

Set this key on quantity samples that represent distance, or on workout segments. Set its value to an HKQuantity object with a percent unit, where 100% indicates a 45 degree slope.

HealthKit assigns this metadata key to the segments it automatically creates for HKWorkoutActivityType.downhillSkiing and HKWorkoutActivityType.snowboarding workout sessions (Apple Watch Series 3 only).

## See Also

### Skiing and Snowboarding

let HKMetadataKeyElevationAscended: String

A key that indicates the cumulative elevation ascended during a workout.

let HKMetadataKeyElevationDescended: String

A key that indicates the cumulative elevation descended during a workout.

