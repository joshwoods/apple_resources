

- SwiftUI
- TimelineSchedule
-  animation 

Type Property

# animation

A pausable schedule of dates updating at a frequency no more quickly than the provided interval.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var animation: AnimationTimelineSchedule { get }
```

Available when `Self` is `AnimationTimelineSchedule`.

## See Also

### Getting built-in schedules

static func animation(minimumInterval: Double?, paused: Bool) -> AnimationTimelineSchedule

A pausable schedule of dates updating at a frequency no more quickly than the provided interval.

static var everyMinute: EveryMinuteTimelineSchedule

A schedule for updating a timeline view at the start of every minute.

static func explicit&lt;S>(S) -> ExplicitTimelineSchedule&lt;S>

A schedule for updating a timeline view at explicit points in time.

static func periodic(from: Date, by: TimeInterval) -> PeriodicTimelineSchedule

A schedule for updating a timeline view at regular intervals.

