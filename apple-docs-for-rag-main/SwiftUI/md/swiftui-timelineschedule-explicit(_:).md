

- SwiftUI
- TimelineSchedule
-  explicit(\_:) 

Type Method

# explicit(\_:)

A schedule for updating a timeline view at explicit points in time.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func explicit(_ dates: S) -> ExplicitTimelineSchedule where Self == ExplicitTimelineSchedule, S : Sequence, S.Element == Date
```

## Parameters 

`dates`  

The sequence of dates at which a timeline view updates. Use a monotonically increasing sequence of dates, and ensure that at least one is in the future.

## Discussion

Initialize a TimelineView with an explicit timeline schedule when you want to schedule view updates at particular points in time:

```
let dates = [
    Date(timeIntervalSinceNow: 10), // Update ten seconds from now,
    Date(timeIntervalSinceNow: 12) // and a few seconds later.
]

struct MyView: View {
    var body: some View {
        TimelineView(.explicit(dates)) { context in
            Text(context.date.description)
        }
    }
}
```

The timeline view updates its content on exactly the dates that you specify, until it runs out of dates, after which it stops changing. If the dates you provide are in the past, the timeline view updates exactly once with the last entry. If you only provide dates in the future, the timeline view renders with the current date until the first date arrives. If you provide one or more dates in the past and one or more in the future, the view renders the most recent past date, refreshing normally on all subsequent dates.

## See Also

### Getting built-in schedules

static var animation: AnimationTimelineSchedule

A pausable schedule of dates updating at a frequency no more quickly than the provided interval.

static func animation(minimumInterval: Double?, paused: Bool) -> AnimationTimelineSchedule

A pausable schedule of dates updating at a frequency no more quickly than the provided interval.

static var everyMinute: EveryMinuteTimelineSchedule

A schedule for updating a timeline view at the start of every minute.

static func periodic(from: Date, by: TimeInterval) -> PeriodicTimelineSchedule

A schedule for updating a timeline view at regular intervals.

