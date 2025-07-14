

- HealthKit
- HKWorkoutEvent
-  init(type:date:) Deprecated

Initializer

# init(type:date:)

Instantiates and returns a new workout event with the specified type and date.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 13.0+visionOS 1.0–1.0DeprecatedwatchOS 2.0–4.0Deprecated

``` source
convenience init(
    type: HKWorkoutEventType,
    date: Date
)
```

Deprecated

Use init(type:dateInterval:metadata:) instead.

## Parameters 

`type`  

The type of workout event. For a description of possible events, see HKWorkoutEventType.

`date`  

The time when the transition occurred. For a pause event, this date indicates the start of the break. For a resume event, this date indicates the end of the break. You must use a date between the starting and ending dates of the workout that you intend to modify.

## Return Value

A new workout event.

## See Also

### Deprecated

convenience init(type: HKWorkoutEventType, date: Date, metadata: [String : Any])

Instantiates and returns a new workout event with the specified type, date, and metadata.

Deprecated

var date: Date

The time when the transition occurred.

Deprecated

