

- HealthKit
- HKWorkoutBuilder
-  workoutConfiguration 

Instance Property

# workoutConfiguration

The configuration information for the workout.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOSvisionOS 1.0+watchOS 5.0+

``` source
@NSCopying
var workoutConfiguration: HKWorkoutConfiguration { get }
```

## See Also

### Creating the builder

init(healthStore: HKHealthStore, configuration: HKWorkoutConfiguration, device: HKDevice?)

Returns a new workout builder object that is not connected to a workout session or other data source.

var device: HKDevice?

The device associated with the workout.

