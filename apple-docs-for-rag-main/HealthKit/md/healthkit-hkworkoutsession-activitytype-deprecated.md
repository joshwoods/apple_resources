

- HealthKit
- HKWorkoutSession
-  activityType Deprecated

Instance Property

# activityType

The workout activity performed during this session.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOSvisionOS 1.0+watchOS 2.0–3.0Deprecated

``` source
var activityType: HKWorkoutActivityType { get }
```

Deprecated

Use workoutConfiguration instead.

## Discussion

For a list of possible activity types, see HKWorkoutActivityType.

## See Also

### Deprecated methods

init(activityType: HKWorkoutActivityType, locationType: HKWorkoutSessionLocationType)

Returns a newly instantiated workout session.

Deprecated

init(configuration: HKWorkoutConfiguration) throws

Returns a newly instantiated workout session.

Deprecated

var locationType: HKWorkoutSessionLocationType

A value that indicates whether the workout session occurred indoors or outdoors.

Deprecated

