

- SwiftUI
-  ExplicitTimelineSchedule 

Structure

# ExplicitTimelineSchedule

A schedule for updating a timeline view at explicit points in time.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct ExplicitTimelineSchedule where Entries : Sequence, Entries.Element == Date
```

## Overview

You can also use explicit(_:) to construct this schedule.

## Topics

### Creating a schedule

init(Entries)

Creates a schedule composed of an explicit sequence of dates.

### Getting the sequence of dates

func entries(from: Date, mode: TimelineScheduleMode) -> Entries

Provides the sequence of dates with which you initialized the schedule.

## Relationships

### Conforms To

- TimelineSchedule

## See Also

### Supporting types

struct AnimationTimelineSchedule

A pausable schedule of dates updating at a frequency no more quickly than the provided interval.

struct EveryMinuteTimelineSchedule

A schedule for updating a timeline view at the start of every minute.

struct PeriodicTimelineSchedule

A schedule for updating a timeline view at regular intervals.

