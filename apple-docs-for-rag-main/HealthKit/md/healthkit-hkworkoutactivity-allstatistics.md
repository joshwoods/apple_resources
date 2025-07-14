

- HealthKit
- HKWorkoutActivity
-  allStatistics 

Instance Property

# allStatistics

A dictionary that contains all the statistics for the activity.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
var allStatistics: [HKQuantityType : HKStatistics] { get }
```

## Discussion

HealthKit calculates an HKStatistics object for each HKQuantityType, based on the HKQuantitySample objects associated with the containing workout, and falling within the workout activity’s time frame.

Furthermore, if a quantity sample extends beyond the activity’s time frame, HealthKit interpolates a quantity value to represent the portion within the time frame, and uses that value instead.

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

func statistics(for: HKQuantityType) -> HKStatistics?

Returns the activity’s statistics for the provided quantity type.

var metadata: [String : Any]?

Metadata that describes the activity.

var workoutConfiguration: HKWorkoutConfiguration

The configuration information for this part of the workout.

var workoutEvents: [HKWorkoutEvent]

An array of events associated with the containing workout and occurring during the activity’s duration.

