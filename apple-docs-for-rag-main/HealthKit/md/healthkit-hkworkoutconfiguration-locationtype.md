

- HealthKit
- HKWorkoutConfiguration
-  locationType 

Instance Property

# locationType

The workout session’s location.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 3.0+

``` source
var locationType: HKWorkoutSessionLocationType { get set }
```

## Discussion

For a list of possible values, see HKWorkoutSessionLocationType.

## See Also

### Session settings

var activityType: HKWorkoutActivityType

The workout session’s activity type.

enum HKWorkoutSessionLocationType

A constant indicating whether the workout session takes place indoors or outdoors.

var swimmingLocationType: HKWorkoutSwimmingLocationType

The workout session’s swimming location.

enum HKWorkoutSwimmingLocationType

The possible locations for swimming.

var lapLength: HKQuantity?

The length of the lap for a workout session.

