

- SwiftUI
-  PeriodicTimelineSchedule 

Structure

# PeriodicTimelineSchedule

A schedule for updating a timeline view at regular intervals.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct PeriodicTimelineSchedule
```

## Overview

You can also use periodic(from:by:) to construct this schedule.

## Topics

### Creating a schedule

init(from: Date, by: TimeInterval)

Creates a periodic update schedule.

### Getting the sequence of dates

func entries(from: Date, mode: TimelineScheduleMode) -> PeriodicTimelineSchedule.Entries

Provides a sequence of periodic dates starting from around a given date.

struct Entries

The sequence of dates in periodic schedule.

## Relationships

### Conforms To

- Sendable
- TimelineSchedule

## See Also

### Supporting types

struct AnimationTimelineSchedule

A pausable schedule of dates updating at a frequency no more quickly than the provided interval.

struct EveryMinuteTimelineSchedule

A schedule for updating a timeline view at the start of every minute.

struct ExplicitTimelineSchedule

A schedule for updating a timeline view at explicit points in time.

