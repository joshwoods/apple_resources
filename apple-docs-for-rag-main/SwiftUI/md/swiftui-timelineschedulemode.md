

- SwiftUI
-  TimelineScheduleMode 

Enumeration

# TimelineScheduleMode

A mode of operation for timeline schedule updates.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum TimelineScheduleMode
```

## Overview

A TimelineView provides a mode when calling its schedule’s entries(from:mode:) method. The view chooses a mode based on the state of the system. For example, a watchOS view might request a lower frequency of updates, using the TimelineScheduleMode.lowFrequency mode, when the user lowers their wrist.

## Topics

### Getting timeline schedule modes

case normal

A mode that produces schedule updates at the schedule’s natural cadence.

case lowFrequency

A mode that produces schedule updates at a reduced rate.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Specifying a mode

typealias Mode

An alias for the timeline schedule update mode.

