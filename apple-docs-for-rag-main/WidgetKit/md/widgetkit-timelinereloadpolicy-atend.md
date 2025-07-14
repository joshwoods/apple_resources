

- WidgetKit
- TimelineReloadPolicy
-  atEnd 

Type Property

# atEnd

A policy that specifies that WidgetKit requests a new timeline after the last date in a timeline passes.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+watchOS 9.0+

``` source
static let atEnd: TimelineReloadPolicy
```

## See Also

### Reload Policies

static func after(Date) -> TimelineReloadPolicy

A policy that specifies a future date for WidgetKit to request a new timeline.

static let never: TimelineReloadPolicy

A policy that specifies that the app prompts WidgetKit when a new timeline is available.

