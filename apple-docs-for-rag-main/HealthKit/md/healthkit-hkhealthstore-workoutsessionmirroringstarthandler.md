

- HealthKit
- HKHealthStore
-  workoutSessionMirroringStartHandler 

Instance Property

# workoutSessionMirroringStartHandler

A block that the system calls when it starts a mirrored workout session.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOSvisionOS 1.0+watchOS 10.0+

``` source
var workoutSessionMirroringStartHandler: ((HKWorkoutSession) -> Void)? { get set }
```

## Discussion

The system calls this block on the companion iPhone when someone starts a mirrored workout on Apple Watch. If your iOS app isn’t active, the system launches it in the background.

```
// The HealthKit store calls this closure when Apple Watch starts a remote session.
store.workoutSessionMirroringStartHandler = { mirroredSession in
    // Reset the health data.
    self.data = HealthData()

    // Save a reference to the workout session.
    self.session = mirroredSession
    logger.debug("*** A session started on the companion Apple Watch. ***")
}
```

To ensure that your app can always catch incoming mirrored workout sessions, assign this property as soon as your app launches.

Important

Your app may receive multiple calls to workoutSessionMirroringStartHandler. If iPhone and Apple Watch lose their connection in the middle of a workout session, Apple Watch automatically tries to reconnect. Each call has its own HKWorkoutSession instance.

The system calls this block from an arbitrary background queue.

## See Also

### Managing workout sessions

func startWatchApp(with: HKWorkoutConfiguration, completion: (Bool, (any Error)?) -> Void)

Launches or wakes the companion watchOS app to create a new workout session.

func pause(HKWorkoutSession)

Pauses the provided workout session.

func resumeWorkoutSession(HKWorkoutSession)

Resumes the provided workout session.

