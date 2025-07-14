

- HealthKit
- HKHealthStore
-  pause(\_:) 

Instance Method

# pause(\_:)

Pauses the provided workout session.

macOSwatchOS 3.0–5.0Deprecated

``` source
func pause(_ workoutSession: HKWorkoutSession)
```

## Parameters 

`workoutSession`  

The workout session to pause.

## Discussion

This method pauses the provided session if it is currently running. The workout session’s state transitions to `HKWorkoutSessionStatePaused`, and the system generates an HKWorkoutEventType.pause event and passes it to the workout session delegate’s `workoutSession:didGenerateEvent:` method.

## See Also

### Managing workout sessions

var workoutSessionMirroringStartHandler: ((HKWorkoutSession) -> Void)?

A block that the system calls when it starts a mirrored workout session.

func startWatchApp(with: HKWorkoutConfiguration, completion: (Bool, (any Error)?) -> Void)

Launches or wakes the companion watchOS app to create a new workout session.

func resumeWorkoutSession(HKWorkoutSession)

Resumes the provided workout session.

