

- HealthKit
- HKWorkoutEventType
-  HKWorkoutEventType.lap 

Case

# HKWorkoutEventType.lap

A constant indicating a lap.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 3.0+

``` source
case lap
```

## Mentioned in 

Running workout sessions

## Discussion

Lap events partition a workout into segments of equal distance (for example, laps around a track or laps in a pool). The lap’s dateInterval property should mark the start and end of the lap. Lap events can’t overlap.

When you receive lap events from the HealthKit store, examine the event’s dateInterval property to interpret the lap correctly:

**Zero-duration intervals.** Older lap events (created before iOS 11 and watchOS 4) have a zero-duration date interval that marks the end of the lap. Each lap is assumed to start when the previous lap ends, and laps fill the entire workout completely.\*\*\*\*

**Nonzero-duration intervals.** Newer lap events use the date interval to mark the start and the duration of the lap. These events have a nonzero duration, and they do not need to fill the workout; however, you should ideally mark any rest periods between laps using HKWorkoutEventType.pause and HKWorkoutEventType.resume events.

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

case segment

A constant indicating a period of time of interest during a workout.

case marker

A constant indicating a point of interest during a workout session.

