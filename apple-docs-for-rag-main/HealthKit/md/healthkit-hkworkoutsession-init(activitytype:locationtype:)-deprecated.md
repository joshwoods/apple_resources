

- HealthKit
- HKWorkoutSession
-  init(activityType:locationType:) Deprecated

Initializer

# init(activityType:locationType:)

Returns a newly instantiated workout session.

watchOS 2.0–3.0Deprecated

``` source
init(
    activityType: HKWorkoutActivityType,
    locationType: HKWorkoutSessionLocationType
)
```

Deprecated

Use init(healthStore:configuration:) instead.

## Parameters 

`activityType`  

The type of activity being performed in the workout. For a list of possible activities, see HKWorkoutActivityType.

`locationType`  

A value indicating whether the workout was performed indoors or outdoors. For a list of possible location values, see HKWorkoutSessionLocationType.

## Return Value

A newly initialized workout session object for the specified activity type and location.

## Discussion

HealthKit uses the session’s workout activity and location type to fine tune Apple Watch’s sensors for the selected activity. All workout sessions generate higher-frequency heart rate samples; however, an outdoor cycling activity generates more accurate location data, while an indoor cycling activity does not.

## See Also

### Deprecated methods

init(configuration: HKWorkoutConfiguration) throws

Returns a newly instantiated workout session.

Deprecated

var activityType: HKWorkoutActivityType

The workout activity performed during this session.

Deprecated

var locationType: HKWorkoutSessionLocationType

A value that indicates whether the workout session occurred indoors or outdoors.

Deprecated

