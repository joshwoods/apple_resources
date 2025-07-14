

- HealthKit
-  HKMetadataKeyMaximumSpeed 

Global Variable

# HKMetadataKeyMaximumSpeed

A key that indicates the maximum speed during a workout.

iOS 11.2+iPadOS 11.2+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 4.2+

``` source
let HKMetadataKeyMaximumSpeed: String
```

## Mentioned in 

Receiving Downhill Skiing and Snowboarding Data

## Discussion

Set this key on a workout, workout segment, or a quantity sample that represents distance. Set its value to an HKQuantity object with a length/time unit (for example, m/s). For more information on creating complex units, see Performing unit math.

HealthKit assigns this metadata key to the segments it automatically creates for HKWorkoutActivityType.downhillSkiing and HKWorkoutActivityType.snowboarding workout sessions (Apple Watch Series 3 only).

## See Also

### Speed

let HKMetadataKeyAverageSpeed: String

A key that indicates the average speed during a workout.

