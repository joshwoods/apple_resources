

- HealthKit
- HKWorkoutEvent
-  init(type:dateInterval:metadata:) 

Initializer

# init(type:dateInterval:metadata:)

Instantiates and returns a new workout event with the specified type, date interval, and metadata.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 4.0+

``` source
convenience init(
    type: HKWorkoutEventType,
    dateInterval: DateInterval,
    metadata: [String : Any]?
)
```

## Parameters 

`type`  

The type of workout event. For a description of possible events, see HKWorkoutEventType.

`dateInterval`  

Most event types support only date intervals with a zero-length duration. These intervals indicate a single point in time, represented by the interval’s startDate property. Only HKWorkoutEventType.lap and HKWorkoutEventType.segment event types support intervals with nonzero durations.

`metadata`  

The metadata associated with the workout event.

## Return Value

A new workout event.

