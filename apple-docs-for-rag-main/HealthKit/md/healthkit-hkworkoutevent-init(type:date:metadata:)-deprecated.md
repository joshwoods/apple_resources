

- HealthKit
- HKWorkoutEvent
-  init(type:date:metadata:) Deprecated

Initializer

# init(type:date:metadata:)

Instantiates and returns a new workout event with the specified type, date, and metadata.

iOS 10.0–11.0DeprecatediPadOS 10.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 13.0+visionOS 1.0–1.0DeprecatedwatchOS 3.0–4.0Deprecated

``` source
convenience init(
    type: HKWorkoutEventType,
    date: Date,
    metadata: [String : Any]
)
```

Deprecated

Use init(type:dateInterval:metadata:) instead.

## Parameters 

`type`  

The type of workout event. For a description of possible events, see HKWorkoutEventType.

`date`  

The time when the transition occurred. For a pause event, this date indicates the start of the break. For a resume event, this date indicates the end of the break. You must use a date between the starting and ending dates of the workout that you intend to modify.

`metadata`  

The metadata associated with the workout event.

## See Also

### Deprecated

convenience init(type: HKWorkoutEventType, date: Date)

Instantiates and returns a new workout event with the specified type and date.

Deprecated

var date: Date

The time when the transition occurred.

Deprecated

