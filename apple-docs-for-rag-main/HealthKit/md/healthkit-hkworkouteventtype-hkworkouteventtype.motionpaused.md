

- HealthKit
- HKWorkoutEventType
-  HKWorkoutEventType.motionPaused 

Case

# HKWorkoutEventType.motionPaused

A constant indicating that the system has automatically paused a workout session.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 3.0+

``` source
case motionPaused
```

## Mentioned in 

Receiving Downhill Skiing and Snowboarding Data

## Discussion

During running workout sessions, Apple Watch can automatically generate motion pause events when the user stops moving. Users can enable or disable this feature using the watch’s Settings \> General \> Workout \> Autopause setting.

## See Also

### Events

case pause

A constant indicating that the workout has paused.

case resume

A constant indicating that the workout has resumed.

case motionResumed

A constant indicating that the system has automatically resumed a workout session.

case pauseOrResumeRequest

A constant indicating that the user has requested a pause or resume.

case lap

A constant indicating a lap.

case segment

A constant indicating a period of time of interest during a workout.

case marker

A constant indicating a point of interest during a workout session.

