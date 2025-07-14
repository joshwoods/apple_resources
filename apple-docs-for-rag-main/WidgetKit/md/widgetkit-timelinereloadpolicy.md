

- WidgetKit
-  TimelineReloadPolicy 

Structure

# TimelineReloadPolicy

A type that indicates the earliest date WidgetKit requests a new timeline from the widget’s provider.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+watchOS 9.0+

``` source
struct TimelineReloadPolicy
```

## Topics

### Reload Policies

static let atEnd: TimelineReloadPolicy

A policy that specifies that WidgetKit requests a new timeline after the last date in a timeline passes.

static func after(Date) -> TimelineReloadPolicy

A policy that specifies a future date for WidgetKit to request a new timeline.

static let never: TimelineReloadPolicy

A policy that specifies that the app prompts WidgetKit when a new timeline is available.

## Relationships

### Conforms To

- Equatable

## See Also

### Getting Timeline Properties

let entries: [EntryType]

An array of timeline entries.

let policy: TimelineReloadPolicy

The policy that determines the earliest date and time WidgetKit requests a new timeline from a timeline provider.

