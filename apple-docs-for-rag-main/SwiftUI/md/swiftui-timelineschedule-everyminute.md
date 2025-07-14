

- SwiftUI
- TimelineSchedule
-  everyMinute 

Type Property

# everyMinute

A schedule for updating a timeline view at the start of every minute.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var everyMinute: EveryMinuteTimelineSchedule { get }
```

Available when `Self` is `EveryMinuteTimelineSchedule`.

## Discussion

Initialize a TimelineView with an every minute timeline schedule when you want to schedule timeline view updates at the start of every minute:

```
TimelineView(.everyMinute) { context in
    Text(context.date.description)
}
```

The schedule provides the first date as the beginning of the minute in which you use it to initialize the timeline view. For example, if you create the timeline view at `10:09:38`, the schedule’s first entry is `10:09:00`. In response, the timeline view performs its first update immediately, providing the beginning of the current minute, namely `10:09:00`, as context to its content. Subsequent updates happen at the beginning of each minute that follows.

The schedule defines the EveryMinuteTimelineSchedule.Entries structure to return the sequence of dates when the timeline view calls the entries(from:mode:) method.

## See Also

### Getting built-in schedules

static var animation: AnimationTimelineSchedule

A pausable schedule of dates updating at a frequency no more quickly than the provided interval.

static func animation(minimumInterval: Double?, paused: Bool) -> AnimationTimelineSchedule

A pausable schedule of dates updating at a frequency no more quickly than the provided interval.

static func explicit&lt;S>(S) -> ExplicitTimelineSchedule&lt;S>

A schedule for updating a timeline view at explicit points in time.

static func periodic(from: Date, by: TimeInterval) -> PeriodicTimelineSchedule

A schedule for updating a timeline view at regular intervals.

