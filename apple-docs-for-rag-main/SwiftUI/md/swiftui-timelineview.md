

- SwiftUI
-  TimelineView 

Structure

# TimelineView

A view that updates according to a schedule that you provide.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct TimelineView where Schedule : TimelineSchedule
```

## Overview

A timeline view acts as a container with no appearance of its own. Instead, it redraws the content it contains at scheduled points in time. For example, you can update the face of an analog timer once per second:

```
TimelineView(.periodic(from: startDate, by: 1)) { context in
    AnalogTimerView(date: context.date)
}
```

The closure that creates the content receives an input of type TimelineView.Context that you can use to customize the content’s appearance. The context includes the date that triggered the update. In the example above, the timeline view sends that date to an analog timer that you create so the timer view knows how to draw the hands on its face.

The context also includes a cadence property that you can use to hide unnecessary detail. For example, you can use the cadence to decide when it’s appropriate to display the timer’s second hand:

```
TimelineView(.periodic(from: startDate, by: 1.0)) { context in
    AnalogTimerView(
        date: context.date,
        showSeconds: context.cadence 

The system might use a cadence that’s slower than the schedule’s update rate. For example, a view on watchOS might remain visible when the user lowers their wrist, but update less frequently, and thus require less detail.

You can define a custom schedule by creating a type that conforms to the TimelineSchedule protocol, or use one of the built-in schedule types:

- Use an everyMinute schedule to update at the beginning of each minute.

- Use a periodic(from:by:) schedule to update periodically with a custom start time and interval between updates.

- Use an explicit(_:) schedule when you need a finite number, or irregular set of updates.

For a schedule containing only dates in the past, the timeline view shows the last date in the schedule. For a schedule containing only dates in the future, the timeline draws its content using the current date until the first scheduled date arrives.

## Topics

### Creating a timeline

init(Schedule, content: (TimelineViewDefaultContext) -> Content)

Creates a new timeline view that uses the given schedule.

struct Context

Information passed to a timeline view’s content callback.

### Deprecated symbols

init(Schedule, content: (TimelineView&lt;Schedule, Content>.Context) -> Content)

Creates a new timeline view that uses the given schedule.

Deprecated

### Initializers

init(_:content:)

Creates a new timeline view that uses the given schedule.

## Relationships

### Conforms To

- Copyable
- View

  Conforms when `Schedule` conforms to `TimelineSchedule` and `Content` conforms to `View`.

## See Also

### Updating a view on a schedule

Updating watchOS apps with timelines

Seamlessly schedule updates to your user interface, even while it’s inactive.

protocol TimelineSchedule

A type that provides a sequence of dates for use as a schedule.

typealias TimelineViewDefaultContext

Information passed to a timeline view’s content callback.

