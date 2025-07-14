

- DeviceActivity
- DeviceActivitySchedule
-  nextInterval 

Instance Property

# nextInterval

The schedule’s next interval or the current interval if one is ongoing.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
var nextInterval: DateInterval? { get }
```

## Discussion

`nil` if `intervalStart` and `intervalEnd` don’t match any future dates. The start and end dates indicate the earliest point when the intervalDidStart(for:) and intervalDidEnd(for:) methods of your app extension’s principal class invokes. The system actually invokes these methods when someone uses the device during the interval. The system additionally calls intervalDidEnd(for:) when you stop monitoring an activity with an ongoing interval. The system doesn’t call these methods unless the device is used during the interval.

Note

This interval is computed using the provided date components and the Calendar.MatchingPolicy.nextTimePreservingSmallerComponents policy for the `calendar` of both date components. If you don’t specify a calendar for either components, the system uses `Calendar.current`. The system bases the interval’s end date on wall-clock time, regardless of any time zone changes that occur during the interval.

## See Also

### Creating a Schedule

init(intervalStart: DateComponents, intervalEnd: DateComponents, repeats: Bool, warningTime: DateComponents?)

Creates a new schedule.

var intervalEnd: DateComponents

The date components that represent the end time for a schedule’s interval.

var intervalStart: DateComponents

The date components that represent the start time for a schedule’s interval.

var repeats: Bool

A Boolean value that indicates whether the schedule recurs.

var warningTime: DateComponents?

Optional components that generate a warning prior to regularly scheduled events.

