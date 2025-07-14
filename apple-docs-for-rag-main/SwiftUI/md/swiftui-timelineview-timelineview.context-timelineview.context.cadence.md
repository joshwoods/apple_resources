

- SwiftUI
- TimelineView
- TimelineView.Context
-  TimelineView.Context.Cadence 

Enumeration

# TimelineView.Context.Cadence

A rate at which timeline views can receive updates.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum Cadence
```

## Overview

Use the cadence presented to content in a TimelineView to hide information that updates faster than the view’s current update rate. For example, you could hide the millisecond component of a digital timer when the cadence is TimelineView.Context.Cadence.seconds or TimelineView.Context.Cadence.minutes.

Because this enumeration conforms to the Comparable protocol, you can compare cadences with relational operators. Slower cadences have higher values, so you could perform the check described above with the following comparison:

```
let hideMilliseconds = cadence > .live
```

## Topics

### Getting cadences

case live

Updates the view continuously.

case seconds

Updates the view approximately once per second.

case minutes

Updates the view approximately once per minute.

## Relationships

### Conforms To

- Comparable
- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Getting the cadence

let cadence: TimelineView&lt;Schedule, Content>.Context.Cadence

The rate at which the timeline updates the view.

