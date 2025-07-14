

- DeviceActivity
- DeviceActivitySchedule
-  init(intervalStart:intervalEnd:repeats:warningTime:) 

Initializer

# init(intervalStart:intervalEnd:repeats:warningTime:)

Creates a new schedule.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
init(
    intervalStart: DateComponents,
    intervalEnd: DateComponents,
    repeats: Bool,
    warningTime: DateComponents? = nil
)
```

## Parameters 

`intervalStart`  

The date components that represent the start time for a schedule’s interval.

`intervalEnd`  

The date components that represent the end time for a schedule’s interval.

`repeats`  

Indicates whether the schedule recurs. If `false`, the extension stops receiving callbacks when the interval ends for the first time.

`warningTime`  

An optional warning time to receive callbacks. If the components specify a longer time interval than the schedule’s interval, the system clamps the warning callbacks for each event’s threshold to the start time of the interval.

## Discussion

Important

If the current date falls in between intervalStart and intervalEnd, the system calls the intervalDidStart(for:) method immediately upon starting to monitor the activity. If the current date doesn’t fall in between `intervalStart` and `intervalEnd`, then `intervalDidStart(for:)` calls at the next date matching `intervalStart`.

## See Also

### Creating a Schedule

var intervalEnd: DateComponents

The date components that represent the end time for a schedule’s interval.

var intervalStart: DateComponents

The date components that represent the start time for a schedule’s interval.

var nextInterval: DateInterval?

The schedule’s next interval or the current interval if one is ongoing.

var repeats: Bool

A Boolean value that indicates whether the schedule recurs.

var warningTime: DateComponents?

Optional components that generate a warning prior to regularly scheduled events.

