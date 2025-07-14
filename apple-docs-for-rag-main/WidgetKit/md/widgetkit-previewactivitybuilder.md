

- WidgetKit
-  PreviewActivityBuilder 

Structure

# PreviewActivityBuilder

iOS 17.0+iPadOS 17.0+

``` source
@resultBuilder
struct PreviewActivityBuilder where A : ActivityAttributes
```

## Topics

### Previewing Live Activities

static func buildArray([[A.ContentState]]) -> [A.ContentState]

static func buildExpression(A.ContentState) -> [A.ContentState]

static func buildPartialBlock(accumulated: [A.ContentState], next: [A.ContentState]) -> [A.ContentState]

static func buildPartialBlock(first: [A.ContentState]) -> [A.ContentState]

## See Also

### Generated structures

struct PreviewTimelineBuilder

