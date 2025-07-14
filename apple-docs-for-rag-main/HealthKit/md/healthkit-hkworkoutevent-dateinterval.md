

- HealthKit
- HKWorkoutEvent
-  dateInterval 

Instance Property

# dateInterval

The time and duration of the event.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 4.0+

``` source
var dateInterval: DateInterval { get }
```

## Discussion

Most event types support only date intervals with a zero-length duration. These intervals indicate a single point in time, represented by the interval’s startDate property. Only HKWorkoutEventType.lap and HKWorkoutEventType.segment event types support intervals with nonzero durations.

## See Also

### Getting property data

var type: HKWorkoutEventType

The type of workout event.

var metadata: [String : Any]?

The metadata associated with the workout event.

