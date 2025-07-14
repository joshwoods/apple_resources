

- HealthKit
- HKWorkoutActivity
-  uuid 

Instance Property

# uuid

The activity’s universally unique identifier (UUID).

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
var uuid: UUID { get }
```

## Discussion

HealthKit assigns a UUID to the workout activity when you create it. If you want to add your own unique ID, add it to the activity’s metadata using the HKMetadataKeyExternalUUID key.

## See Also

### Accessing workout data

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

