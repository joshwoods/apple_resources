

- DeviceActivity
- DeviceActivitySchedule
-  repeats 

Instance Property

# repeats

A Boolean value that indicates whether the schedule recurs.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
var repeats: Bool { get }
```

## Discussion

Use `repeats` to create an activity schedule that repeats until the activity-monitoring stops.

## See Also

### Creating a Schedule

init(intervalStart: DateComponents, intervalEnd: DateComponents, repeats: Bool, warningTime: DateComponents?)

Creates a new schedule.

var intervalEnd: DateComponents

The date components that represent the end time for a schedule’s interval.

var intervalStart: DateComponents

The date components that represent the start time for a schedule’s interval.

var nextInterval: DateInterval?

The schedule’s next interval or the current interval if one is ongoing.

var warningTime: DateComponents?

Optional components that generate a warning prior to regularly scheduled events.

