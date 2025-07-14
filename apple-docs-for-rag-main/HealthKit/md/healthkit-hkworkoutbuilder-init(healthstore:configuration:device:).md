

- HealthKit
- HKWorkoutBuilder
-  init(healthStore:configuration:device:) 

Initializer

# init(healthStore:configuration:device:)

Returns a new workout builder object that is not connected to a workout session or other data source.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOSvisionOS 1.0+watchOS 5.0+

``` source
init(
    healthStore: HKHealthStore,
    configuration: HKWorkoutConfiguration,
    device: HKDevice?
)
```

## See Also

### Creating the builder

var device: HKDevice?

The device associated with the workout.

var workoutConfiguration: HKWorkoutConfiguration

The configuration information for the workout.

