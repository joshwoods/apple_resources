

- HealthKit
- HKWorkoutActivity
-  statistics(for:) 

Instance Method

# statistics(for:)

Returns the activity’s statistics for the provided quantity type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
func statistics(for quantityType: HKQuantityType) -> HKStatistics?
```

## Parameters 

`quantityType`  

The type of HKQuantitySample objects used to calculate the statistics.

## Discussion

HealthKit calculates an HKStatistics object based on the HKQuantitySample objects that meet the following requirements:

- Match the specified HKQuantityType.

- Are associated with the containing workout.

- Fall within the activity’s time frame.

Furthermore, if a quantity sample extends beyond the activity’s time frame, HealthKit interpolates a quantity value to represent the portion within the time frame, and uses that value instead.

If there are no matching quantity values, this method returns `nil`.

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

var metadata: [String : Any]?

Metadata that describes the activity.

var workoutConfiguration: HKWorkoutConfiguration

The configuration information for this part of the workout.

var workoutEvents: [HKWorkoutEvent]

An array of events associated with the containing workout and occurring during the activity’s duration.

