

- HealthKit
- HKHealthStore
-  relateWorkoutEffortSample(\_:with:activity:completion:) 

Instance Method

# relateWorkoutEffortSample(\_:with:activity:completion:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+watchOS 11.0+

``` source
func relateWorkoutEffortSample(
    _ sample: HKSample,
    with workout: HKWorkout,
    activity: HKWorkoutActivity?,
    completion: @escaping (Bool, (any Error)?) -> Void
)
```

``` source
func relateWorkoutEffortSample(
    _ sample: HKSample,
    with workout: HKWorkout,
    activity: HKWorkoutActivity?
) async throws -> Bool
```

