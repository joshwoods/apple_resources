

- SwiftUI
-  AnimationTimelineSchedule 

Structure

# AnimationTimelineSchedule

A pausable schedule of dates updating at a frequency no more quickly than the provided interval.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct AnimationTimelineSchedule
```

## Overview

You can also use animation(minimumInterval:paused:) to construct this schedule.

## Topics

### Creating a schedule

init(minimumInterval: Double?, paused: Bool)

Create a pausable schedule of dates updating at a frequency no more quickly than the provided interval.

### Getting the sequence of dates

func entries(from: Date, mode: TimelineScheduleMode) -> AnimationTimelineSchedule.Entries

Returns entries at the frequency of the animation schedule.

## Relationships

### Conforms To

- Sendable
- TimelineSchedule

## See Also

### Supporting types

struct EveryMinuteTimelineSchedule

A schedule for updating a timeline view at the start of every minute.

struct ExplicitTimelineSchedule

A schedule for updating a timeline view at explicit points in time.

struct PeriodicTimelineSchedule

A schedule for updating a timeline view at regular intervals.

