

- HealthKit
-  HKMetadataKeyElevationDescended 

Global Variable

# HKMetadataKeyElevationDescended

A key that indicates the cumulative elevation descended during a workout.

iOS 11.2+iPadOS 11.2+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 4.2+

``` source
let HKMetadataKeyElevationDescended: String
```

## Mentioned in 

Receiving Downhill Skiing and Snowboarding Data

## Discussion

Set this key on a workout, workout segment, or a quantity sample that represents distance. Set its value to an HKQuantity object with a length unit.

HealthKit assigns this metadata key to the segments it automatically creates for HKWorkoutActivityType.downhillSkiing and HKWorkoutActivityType.snowboarding workout sessions (Apple Watch Series 3 only).

## See Also

### Skiing and Snowboarding

let HKMetadataKeyAlpineSlopeGrade: String

A key that indicates the percent slope of a ski run.

let HKMetadataKeyElevationAscended: String

A key that indicates the cumulative elevation ascended during a workout.

