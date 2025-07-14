

- HealthKit
- HKWorkoutActivity
-  workoutEvents 

Instance Property

# workoutEvents

An array of events associated with the containing workout and occurring during the activity’s duration.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
var workoutEvents: [HKWorkoutEvent] { get }
```

## Discussion

HealthKit sorts the events in ascending order. These events are a subset of the containing workout’s events, that take place between the activity’s startDate and endDate. This includes any event that partially overlaps the activity. As a result, these events may appear in more than one activity.

## See Also

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

