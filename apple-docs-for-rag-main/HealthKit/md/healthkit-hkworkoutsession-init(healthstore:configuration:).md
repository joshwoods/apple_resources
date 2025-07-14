

- HealthKit
- HKWorkoutSession
-  init(healthStore:configuration:) 

Initializer

# init(healthStore:configuration:)

Returns a newly instantiated workout session with an associated workout builder.

watchOS 5.0+

``` source
init(
    healthStore: HKHealthStore,
    configuration workoutConfiguration: HKWorkoutConfiguration
) throws
```

## See Also

### Related Documentation

func associatedWorkoutBuilder() -> HKLiveWorkoutBuilder

Returns the live workout builder associated with the workout session.

