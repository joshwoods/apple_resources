

- HealthKit
- HKWorkoutSession
-  locationType Deprecated

Instance Property

# locationType

A value that indicates whether the workout session occurred indoors or outdoors.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOSvisionOS 1.0+watchOS 2.0–3.0Deprecated

``` source
var locationType: HKWorkoutSessionLocationType { get }
```

Deprecated

Use workoutConfiguration instead.

## Discussion

For a list of possible location values, see HKWorkoutSessionLocationType.

## See Also

### Deprecated methods

init(activityType: HKWorkoutActivityType, locationType: HKWorkoutSessionLocationType)

Returns a newly instantiated workout session.

Deprecated

init(configuration: HKWorkoutConfiguration) throws

Returns a newly instantiated workout session.

Deprecated

var activityType: HKWorkoutActivityType

The workout activity performed during this session.

Deprecated

