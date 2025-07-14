

- DeviceActivity
- DeviceActivitySchedule
-  intervalEnd 

Instance Property

# intervalEnd

The date components that represent the end time for a schedule’s interval.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
var intervalEnd: DateComponents { get }
```

## Discussion

The system uses these components to compute `nextInterval.end`.

## See Also

### Creating a Schedule

init(intervalStart: DateComponents, intervalEnd: DateComponents, repeats: Bool, warningTime: DateComponents?)

Creates a new schedule.

var intervalStart: DateComponents

The date components that represent the start time for a schedule’s interval.

var nextInterval: DateInterval?

The schedule’s next interval or the current interval if one is ongoing.

var repeats: Bool

A Boolean value that indicates whether the schedule recurs.

var warningTime: DateComponents?

Optional components that generate a warning prior to regularly scheduled events.

