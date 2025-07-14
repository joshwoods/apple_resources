

- HealthKit
- HKWorkoutEventType
-  HKWorkoutEventType.motionResumed 

Case

# HKWorkoutEventType.motionResumed

A constant indicating that the system has automatically resumed a workout session.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 3.0+

``` source
case motionResumed
```

## Mentioned in 

Receiving Downhill Skiing and Snowboarding Data

## Discussion

If the system has automatically paused a running workout session, it also generates a motion resumed event when the user starts moving again.

## See Also

### Events

case pause

A constant indicating that the workout has paused.

case resume

A constant indicating that the workout has resumed.

case motionPaused

A constant indicating that the system has automatically paused a workout session.

case pauseOrResumeRequest

A constant indicating that the user has requested a pause or resume.

case lap

A constant indicating a lap.

case segment

A constant indicating a period of time of interest during a workout.

case marker

A constant indicating a point of interest during a workout session.

