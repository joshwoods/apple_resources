

- HealthKit
- HKWorkoutEvent
-  date Deprecated

Instance Property

# date

The time when the transition occurred.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 13.0+visionOS 1.0–1.0DeprecatedwatchOS 2.0–4.0Deprecated

``` source
var date: Date { get }
```

Deprecated

Use dateInterval instead.

## Discussion

For a pause event, this date indicates the start of the break. For a resume event, this date indicates the end of the break. You must use a date between the starting and ending dates of the workout that you intend to modify.

## See Also

### Deprecated

convenience init(type: HKWorkoutEventType, date: Date)

Instantiates and returns a new workout event with the specified type and date.

Deprecated

convenience init(type: HKWorkoutEventType, date: Date, metadata: [String : Any])

Instantiates and returns a new workout event with the specified type, date, and metadata.

Deprecated

