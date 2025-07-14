

- HealthKit
- HKHealthStore
-  end(\_:) Deprecated

Instance Method

# end(\_:)

Ends a workout session for the current app.

watchOS 2.0–5.0Deprecated

``` source
func end(_ workoutSession: HKWorkoutSession)
```

Deprecated

Use HKWorkoutSession's end method

## Parameters 

`workoutSession`  

A currently running workout session. If the session is not running, the system returns an invalidArgumentException exception.

## Discussion

This method returns immediately; however, the work is performed asynchronously on an anonymous serial background queue. If successful, the session’s state transitions to HKWorkoutSessionState.ended, and the system calls the session delegate’s workoutSession(_:didChangeTo:from:date:) method.

## See Also

### Deprecated symbols

func add([HKSample], to: HKWorkout, completion: (Bool, (any Error)?) -> Void)

Associates the provided samples with the specified workout.

Deprecated

func start(HKWorkoutSession)

Starts a workout session for the current app.

Deprecated

