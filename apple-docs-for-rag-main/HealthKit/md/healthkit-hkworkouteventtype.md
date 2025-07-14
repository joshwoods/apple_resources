

- HealthKit
-  HKWorkoutEventType 

Enumeration

# HKWorkoutEventType

Constants that represent events occurring during a workout.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
enum HKWorkoutEventType
```

## Topics

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

case segment

A constant indicating a period of time of interest during a workout.

case marker

A constant indicating a point of interest during a workout session.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

