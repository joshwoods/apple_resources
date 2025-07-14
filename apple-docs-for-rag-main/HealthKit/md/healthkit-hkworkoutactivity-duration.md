

- HealthKit
- HKWorkoutActivity
-  duration 

Instance Property

# duration

The activity’s duration, measured in seconds.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
var duration: TimeInterval { get }
```

## Discussion

HealthKit calculates the duration as the elapsed time between the activity’s startDate and endDate, ignoring any pause periods. If an activity is currently in progress, it has a `nil`-valued endDate. In this case, HealthKit calculates the duration as the time between the startDate and the current time, ignoring any pause periods.

## See Also

### Accessing workout data

var uuid: UUID

The activity’s universally unique identifier (UUID).

var startDate: Date

The activitiy’s start date and time.

var endDate: Date?

The activity’s end date and time.

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

