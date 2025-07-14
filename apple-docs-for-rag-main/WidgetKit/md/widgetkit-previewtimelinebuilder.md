

- WidgetKit
-  PreviewTimelineBuilder 

Structure

# PreviewTimelineBuilder

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+watchOS 10.0+

``` source
@resultBuilder
struct PreviewTimelineBuilder
```

## Topics

### Previewing timelines

static func buildArray([[any TimelineEntry]]) -> [any TimelineEntry]

static func buildExpression(some TimelineEntry) -> [any TimelineEntry]

static func buildPartialBlock(accumulated: [any TimelineEntry], next: [any TimelineEntry]) -> [any TimelineEntry]

static func buildPartialBlock(first: [any TimelineEntry]) -> [any TimelineEntry]

## See Also

### Generated structures

struct PreviewActivityBuilder

