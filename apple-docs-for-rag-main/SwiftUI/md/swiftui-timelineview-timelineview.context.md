

- SwiftUI
- TimelineView
-  TimelineView.Context 

Structure

# TimelineView.Context

Information passed to a timeline view’s content callback.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Context
```

## Overview

The context includes both the date from the schedule that triggered the callback, and a cadence that you can use to customize the appearance of your view. For example, you might choose to display the second hand of an analog clock only when the cadence is TimelineView.Context.Cadence.seconds or faster.

## Topics

### Getting the date

let date: Date

The date from the schedule that triggered the current view update.

### Getting the cadence

let cadence: TimelineView&lt;Schedule, Content>.Context.Cadence

The rate at which the timeline updates the view.

enum Cadence

A rate at which timeline views can receive updates.

### Invalidating the context

func invalidateTimelineContent()

Resets any pre-rendered views the system has from the timeline.

## See Also

### Creating a timeline

init(Schedule, content: (TimelineViewDefaultContext) -> Content)

Creates a new timeline view that uses the given schedule.

