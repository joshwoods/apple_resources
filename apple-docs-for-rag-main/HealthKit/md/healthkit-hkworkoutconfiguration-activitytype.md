

- HealthKit
- HKWorkoutConfiguration
-  activityType 

Instance Property

# activityType

The workout session’s activity type.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 3.0+

``` source
var activityType: HKWorkoutActivityType { get set }
```

## Discussion

For a list of possible values, see HKWorkoutActivityType.

## See Also

### Session settings

var locationType: HKWorkoutSessionLocationType

The workout session’s location.

enum HKWorkoutSessionLocationType

A constant indicating whether the workout session takes place indoors or outdoors.

var swimmingLocationType: HKWorkoutSwimmingLocationType

The workout session’s swimming location.

enum HKWorkoutSwimmingLocationType

The possible locations for swimming.

var lapLength: HKQuantity?

The length of the lap for a workout session.

