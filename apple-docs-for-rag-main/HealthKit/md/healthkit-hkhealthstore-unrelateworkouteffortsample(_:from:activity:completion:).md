

- HealthKit
- HKHealthStore
-  unrelateWorkoutEffortSample(\_:from:activity:completion:) 

Instance Method

# unrelateWorkoutEffortSample(\_:from:activity:completion:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+watchOS 11.0+

``` source
func unrelateWorkoutEffortSample(
    _ sample: HKSample,
    from workout: HKWorkout,
    activity: HKWorkoutActivity?,
    completion: @escaping (Bool, (any Error)?) -> Void
)
```

``` source
func unrelateWorkoutEffortSample(
    _ sample: HKSample,
    from workout: HKWorkout,
    activity: HKWorkoutActivity?
) async throws -> Bool
```

