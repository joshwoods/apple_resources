

- DeviceActivity
- DeviceActivitySchedule
-  warningTime 

Instance Property

# warningTime

Optional components that generate a warning prior to regularly scheduled events.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
var warningTime: DateComponents? { get }
```

## Discussion

You can create a warning time to notify your app extension ahead of time before the scheduled activity begins and ends. For instance, when your app schedules activity-monitoring from 10 a.m. to 11 a.m. for an event with a 30-minute threshold, setting the schedule’s warning time to 5 minutes results in the extension receiving intervalWillStartWarning(for:), intervalWillEndWarning(for:), and eventWillReachThresholdWarning(_:activity:) callbacks at 9:55 a.m., 10:55 a.m, and when 25 minutes of the event’s activity occurs, respectively. If the components specify a longer time interval than the schedule’s interval, the system clamps the warning callbacks for each event’s threshold to the start time of the interval.

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

var repeats: Bool

A Boolean value that indicates whether the schedule recurs.

