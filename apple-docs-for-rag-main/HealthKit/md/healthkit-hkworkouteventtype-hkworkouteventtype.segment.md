

- HealthKit
- HKWorkoutEventType
-  HKWorkoutEventType.segment 

Case

# HKWorkoutEventType.segment

A constant indicating a period of time of interest during a workout.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 4.0+

``` source
case segment
```

## Discussion

Use segments to highlight important time periods during a workout. For example, you could use different segments to mark when a runner is going up or downhill. Similarly, when swimming, you can use segments to group consecutive laps with the same style of stroke.

Unlike laps, segments can freely overlap.

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

case pauseOrResumeRequest

A constant indicating that the user has requested a pause or resume.

case lap

A constant indicating a lap.

case marker

A constant indicating a point of interest during a workout session.

