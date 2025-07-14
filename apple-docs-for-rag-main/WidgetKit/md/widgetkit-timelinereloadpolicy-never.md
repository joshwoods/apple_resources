

- WidgetKit
- TimelineReloadPolicy
-  never 

Type Property

# never

A policy that specifies that the app prompts WidgetKit when a new timeline is available.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+watchOS 9.0+

``` source
static let never: TimelineReloadPolicy
```

## See Also

### Reload Policies

static let atEnd: TimelineReloadPolicy

A policy that specifies that WidgetKit requests a new timeline after the last date in a timeline passes.

static func after(Date) -> TimelineReloadPolicy

A policy that specifies a future date for WidgetKit to request a new timeline.

