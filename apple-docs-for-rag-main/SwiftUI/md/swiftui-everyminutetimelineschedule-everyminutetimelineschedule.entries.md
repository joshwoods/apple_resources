

- SwiftUI
- EveryMinuteTimelineSchedule
-  EveryMinuteTimelineSchedule.Entries 

Structure

# EveryMinuteTimelineSchedule.Entries

The sequence of dates in an every minute schedule.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Entries
```

## Overview

The entries(from:mode:) method returns a value of this type, which is a Sequence of dates, one per minute, in ascending order. A TimelineView that you create updates its content at the moments in time corresponding to the dates included in the sequence.

## Relationships

### Conforms To

- IteratorProtocol
- Sendable
- Sequence

## See Also

### Getting the sequence of dates

func entries(from: Date, mode: TimelineScheduleMode) -> EveryMinuteTimelineSchedule.Entries

Provides a sequence of per-minute dates starting from a given date.

