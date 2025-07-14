

- HealthKit
- HKHealthStore
-  recoverActiveWorkoutSession(completion:) 

Instance Method

# recoverActiveWorkoutSession(completion:)

Recovers an active workout session.

watchOS 5.0+

``` source
func recoverActiveWorkoutSession(completion: @escaping (HKWorkoutSession?, (any Error)?) -> Void)
```

``` source
func recoverActiveWorkoutSession() async throws -> HKWorkoutSession?
```

## Mentioned in 

Running workout sessions

## Discussion

If your app crashes during an active workout session, the system calls your extension delegate’s handleActiveWorkoutRecovery() method the next time your app launches. To recover the workout session, call recoverActiveWorkoutSession(completion:) from your extension delegate’s handleActiveWorkoutRecovery() method. HealthKit then attempts to restore the previous workout session, returning either a new session object or an error to the completion block.

As soon as you receive the session object, you must access its builder and set up your data source and delegates again, as described in Start a session.

## See Also

### Managing workouts

func splitTotalEnergy(HKQuantity, start: Date, end: Date, resultsHandler: (HKQuantity?, HKQuantity?, (any Error)?) -> Void)

Calculates the active and resting energy burned based on the total energy burned over the given duration.

Deprecated

