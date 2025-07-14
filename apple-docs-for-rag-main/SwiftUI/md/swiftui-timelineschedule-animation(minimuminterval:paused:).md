

- SwiftUI
- TimelineSchedule
-  animation(minimumInterval:paused:) 

Type Method

# animation(minimumInterval:paused:)

A pausable schedule of dates updating at a frequency no more quickly than the provided interval.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func animation(
    minimumInterval: Double? = nil,
    paused: Bool = false
) -> AnimationTimelineSchedule
```

Available when `Self` is `AnimationTimelineSchedule`.

## Parameters 

`minimumInterval`  

The minimum interval to update the schedule at. Pass nil to let the system pick an appropriate update interval.

`paused`  

If the schedule should stop generating updates.

## See Also

### Getting built-in schedules

static var animation: AnimationTimelineSchedule

A pausable schedule of dates updating at a frequency no more quickly than the provided interval.

static var everyMinute: EveryMinuteTimelineSchedule

A schedule for updating a timeline view at the start of every minute.

static func explicit&lt;S>(S) -> ExplicitTimelineSchedule&lt;S>

A schedule for updating a timeline view at explicit points in time.

static func periodic(from: Date, by: TimeInterval) -> PeriodicTimelineSchedule

A schedule for updating a timeline view at regular intervals.

