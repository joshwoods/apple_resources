

- HealthKit
- HKHealthStore
-  resumeWorkoutSession(\_:) 

Instance Method

# resumeWorkoutSession(\_:)

Resumes the provided workout session.

macOSwatchOS 3.0–5.0Deprecated

``` source
func resumeWorkoutSession(_ workoutSession: HKWorkoutSession)
```

## Parameters 

`workoutSession`  

The workout session to resume.

## Discussion

This method resumes the provided session if it is currently paused. The workout session’s state transitions to HKWorkoutSessionState.running, and the system generates an HKWorkoutEventType.resume event and passes it to the workout session delegate’s `workoutSession:didGenerateEvent:` method.

## See Also

### Managing workout sessions

var workoutSessionMirroringStartHandler: ((HKWorkoutSession) -> Void)?

A block that the system calls when it starts a mirrored workout session.

func startWatchApp(with: HKWorkoutConfiguration, completion: (Bool, (any Error)?) -> Void)

Launches or wakes the companion watchOS app to create a new workout session.

func pause(HKWorkoutSession)

Pauses the provided workout session.

