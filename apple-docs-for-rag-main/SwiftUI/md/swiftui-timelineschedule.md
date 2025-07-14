

- SwiftUI
-  TimelineSchedule 

Protocol

# TimelineSchedule

A type that provides a sequence of dates for use as a schedule.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
protocol TimelineSchedule
```

## Overview

Types that conform to this protocol implement a particular kind of schedule by defining an entries(from:mode:) method that returns a sequence of dates. Use a timeline schedule type when you initialize a TimelineView. For example, you can create a timeline view that updates every second, starting from some `startDate`, using a periodic schedule returned by periodic(from:by:):

```
TimelineView(.periodic(from: startDate, by: 1.0)) { context in
    // View content goes here.
}
```

You can also create custom timeline schedules. The timeline view updates its content according to the sequence of dates produced by the schedule.

## Topics

### Getting built-in schedules

static var animation: AnimationTimelineSchedule

A pausable schedule of dates updating at a frequency no more quickly than the provided interval.

static func animation(minimumInterval: Double?, paused: Bool) -> AnimationTimelineSchedule

A pausable schedule of dates updating at a frequency no more quickly than the provided interval.

static var everyMinute: EveryMinuteTimelineSchedule

A schedule for updating a timeline view at the start of every minute.

static func explicit&lt;S>(S) -> ExplicitTimelineSchedule&lt;S>

A schedule for updating a timeline view at explicit points in time.

static func periodic(from: Date, by: TimeInterval) -> PeriodicTimelineSchedule

A schedule for updating a timeline view at regular intervals.

### Getting a sequence of dates

func entries(from: Date, mode: Self.Mode) -> Self.Entries

Provides a sequence of dates starting around a given date.

**Required**

associatedtype Entries : Sequence

The sequence of dates within a schedule.

**Required**

### Specifying a mode

typealias Mode

An alias for the timeline schedule update mode.

enum TimelineScheduleMode

A mode of operation for timeline schedule updates.

### Supporting types

struct AnimationTimelineSchedule

A pausable schedule of dates updating at a frequency no more quickly than the provided interval.

struct EveryMinuteTimelineSchedule

A schedule for updating a timeline view at the start of every minute.

struct ExplicitTimelineSchedule

A schedule for updating a timeline view at explicit points in time.

struct PeriodicTimelineSchedule

A schedule for updating a timeline view at regular intervals.

## Relationships

### Conforming Types

- AnimationTimelineSchedule
- EveryMinuteTimelineSchedule
- ExplicitTimelineSchedule
- PeriodicTimelineSchedule

## See Also

### Updating a view on a schedule

Updating watchOS apps with timelines

Seamlessly schedule updates to your user interface, even while it’s inactive.

struct TimelineView

A view that updates according to a schedule that you provide.

typealias TimelineViewDefaultContext

Information passed to a timeline view’s content callback.

