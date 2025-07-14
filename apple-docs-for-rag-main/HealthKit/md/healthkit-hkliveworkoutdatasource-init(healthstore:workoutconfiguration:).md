

- HealthKit
- HKLiveWorkoutDataSource
-  init(healthStore:workoutConfiguration:) 

Initializer

# init(healthStore:workoutConfiguration:)

Creates a new data source based on the provided workout configuration.

macOSwatchOS 5.0+

``` source
init(
    healthStore: HKHealthStore,
    workoutConfiguration configuration: HKWorkoutConfiguration?
)
```

## See Also

### Creating a live data source

var typesToCollect: Set&lt;HKQuantityType>

The quantity type samples that the data source automatically sends to the workout builder.

