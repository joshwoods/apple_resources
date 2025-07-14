

- HealthKit
-  HKWorkoutSessionType 

Enumeration

# HKWorkoutSessionType

The type of session.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOSvisionOS 1.0+watchOS 10.0+

``` source
enum HKWorkoutSessionType
```

## Topics

### Types

case mirrored

A mirrored session, running on the companion iOS device.

case primary

A primary session running on watchOS.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Samples

Adding samples to a workout

Create associated samples that add details to a workout.

Accessing condensed workout samples

Read series data from condensed workouts.

Dividing a HealthKit workout into activities

Partition multisport and interval workouts into activities that represent the different parts of the workout.

class HKWorkout

A workout sample that stores information about a single physical activity.

class HKWorkoutActivity

An object that describes an activity within a longer workout.

class HKWorkoutBuilder

A builder object that incrementally constructs a workout.

class HKWorkoutType

A type that identifies samples that store information about a workout.

let HKWorkoutTypeIdentifier: String

The workout type identifier.

enum HKWorkoutActivityType

The type of activity performed during a workout.

class HKWorkoutEvent

An object representing an important event during a workout.

