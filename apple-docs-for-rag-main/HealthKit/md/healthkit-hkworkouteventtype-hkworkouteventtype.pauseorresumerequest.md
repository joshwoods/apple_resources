

- HealthKit
- HKWorkoutEventType
-  HKWorkoutEventType.pauseOrResumeRequest 

Case

# HKWorkoutEventType.pauseOrResumeRequest

A constant indicating that the user has requested a pause or resume.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 4.0+

``` source
case pauseOrResumeRequest
```

## Discussion

During a workout session, the user can request a pause or resume by pressing both watch buttons. When you receive this event, pause or resume your app’s current workout session.

## See Also

### Events

case pause

A constant indicating that the workout has paused.

case resume

A constant indicating that the workout has resumed.

case motionPaused

A constant indicating that the system has automatically paused a workout session.

case motionResumed

A constant indicating that the system has automatically resumed a workout session.

case lap

A constant indicating a lap.

case segment

A constant indicating a period of time of interest during a workout.

case marker

A constant indicating a point of interest during a workout session.

