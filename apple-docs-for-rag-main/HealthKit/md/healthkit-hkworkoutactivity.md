

- HealthKit
-  HKWorkoutActivity 

Class

# HKWorkoutActivity

An object that describes an activity within a longer workout.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
class HKWorkoutActivity
```

## Mentioned in 

Dividing a HealthKit workout into activities

## Overview

Workout activity objects partition a workout into a set of separate activities. For example, you can use workout activities to record the swim, bike, and running portions of a multisport event, like a triathlon, or to represent the active and rest periods during interval training. All HKWorkout instance have at least one, associated HKWorkoutActivity. If you don’t explicitly set workout activities, HealthKit assigns a workout activity that matches the HKWorkout object’s activity type. For more information, see Dividing a HealthKit workout into activities.

## Topics

### Creating workout activities

init(workoutConfiguration: HKWorkoutConfiguration, start: Date, end: Date?, metadata: [String : Any]?)

Creates a workout activity using the provided configuration, start date, end date, and metadata.

### Accessing workout data

var uuid: UUID

The activity’s universally unique identifier (UUID).

var startDate: Date

The activitiy’s start date and time.

var endDate: Date?

The activity’s end date and time.

var duration: TimeInterval

The activity’s duration, measured in seconds.

var allStatistics: [HKQuantityType : HKStatistics]

A dictionary that contains all the statistics for the activity.

func statistics(for: HKQuantityType) -> HKStatistics?

Returns the activity’s statistics for the provided quantity type.

var metadata: [String : Any]?

Metadata that describes the activity.

var workoutConfiguration: HKWorkoutConfiguration

The configuration information for this part of the workout.

var workoutEvents: [HKWorkoutEvent]

An array of events associated with the containing workout and occurring during the activity’s duration.

### Specifying predicate key paths

let HKPredicateKeyPathWorkoutActivity: String

The key path for accessing a specific workout activity.

let HKPredicateKeyPathWorkoutActivityType: String

The key path for accessing activities that match a workout activity type.

let HKPredicateKeyPathWorkoutActivityStartDate: String

The key path for accessing activities with a matching start date.

let HKPredicateKeyPathWorkoutActivityEndDate: String

The key path for accessing activities with a matching end date.

let HKPredicateKeyPathWorkoutActivityDuration: String

The key path for accessing activities with a matching duration.

let HKPredicateKeyPathWorkoutActivityAverageQuantity: String

The key path for accessing activities with a matching average quantity.

let HKPredicateKeyPathWorkoutActivityMaximumQuantity: String

The key path for accessing activities with a matching maximum quantity.

let HKPredicateKeyPathWorkoutActivityMinimumQuantity: String

The key path for accessing activities with a matching minimum quantity.

let HKPredicateKeyPathWorkoutActivitySumQuantity: String

The key path for accessing activities with a matching sum.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
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

class HKWorkoutBuilder

A builder object that incrementally constructs a workout.

class HKWorkoutType

A type that identifies samples that store information about a workout.

let HKWorkoutTypeIdentifier: String

The workout type identifier.

enum HKWorkoutActivityType

The type of activity performed during a workout.

enum HKWorkoutSessionType

The type of session.

class HKWorkoutEvent

An object representing an important event during a workout.

