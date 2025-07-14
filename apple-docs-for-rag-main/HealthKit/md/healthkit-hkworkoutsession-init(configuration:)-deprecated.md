

- HealthKit
- HKWorkoutSession
-  init(configuration:) Deprecated

Initializer

# init(configuration:)

Returns a newly instantiated workout session.

watchOS 3.0–5.0Deprecated

``` source
init(configuration workoutConfiguration: HKWorkoutConfiguration) throws
```

Deprecated

Use init(healthStore:configuration:) instead.

## Parameters 

`workoutConfiguration`  

A workout configuration object containing the configuration data for this workout session.

## Return Value

A newly initialized workout session object, or `nil` if an error occurred.

## Discussion

HealthKit uses the session’s configuration data to fine tune Apple Watch’s sensors for the selected activity. All workout sessions generate higher-frequency heart rate samples; however, an outdoor cycling activity generates more accurate location data, while an indoor cycling activity does not.

## See Also

### Deprecated methods

init(activityType: HKWorkoutActivityType, locationType: HKWorkoutSessionLocationType)

Returns a newly instantiated workout session.

Deprecated

var activityType: HKWorkoutActivityType

The workout activity performed during this session.

Deprecated

var locationType: HKWorkoutSessionLocationType

A value that indicates whether the workout session occurred indoors or outdoors.

Deprecated

