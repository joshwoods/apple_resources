

- HealthKit
- HKWorkoutActivity
-  endDate 

Instance Property

# endDate

The activity’s end date and time.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
var endDate: Date? { get }
```

## Discussion

While a workout activity is in progress, this value is `nil`. When set to a non-`nil` value, the end date must be equal to or later than its start date.

## See Also

### Accessing workout data

var uuid: UUID

The activity’s universally unique identifier (UUID).

var startDate: Date

The activitiy’s start date and time.

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

