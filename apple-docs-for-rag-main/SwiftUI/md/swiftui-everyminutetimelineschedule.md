

- SwiftUI
-  EveryMinuteTimelineSchedule 

Structure

# EveryMinuteTimelineSchedule

A schedule for updating a timeline view at the start of every minute.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct EveryMinuteTimelineSchedule
```

## Overview

You can also use everyMinute to construct this schedule.

## Topics

### Creating a schedule

init()

Creates a per-minute update schedule.

### Getting the sequence of dates

func entries(from: Date, mode: TimelineScheduleMode) -> EveryMinuteTimelineSchedule.Entries

Provides a sequence of per-minute dates starting from a given date.

struct Entries

The sequence of dates in an every minute schedule.

## Relationships

### Conforms To

- Sendable
- TimelineSchedule

## See Also

### Supporting types

struct AnimationTimelineSchedule

A pausable schedule of dates updating at a frequency no more quickly than the provided interval.

struct ExplicitTimelineSchedule

A schedule for updating a timeline view at explicit points in time.

struct PeriodicTimelineSchedule

A schedule for updating a timeline view at regular intervals.

