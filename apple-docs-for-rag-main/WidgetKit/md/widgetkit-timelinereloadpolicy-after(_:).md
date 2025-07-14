

- WidgetKit
- TimelineReloadPolicy
-  after(\_:) 

Type Method

# after(\_:)

A policy that specifies a future date for WidgetKit to request a new timeline.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+watchOS 9.0+

``` source
static func after(_ date: Date) -> TimelineReloadPolicy
```

## Mentioned in 

Keeping a widget up to date

## See Also

### Reload Policies

static let atEnd: TimelineReloadPolicy

A policy that specifies that WidgetKit requests a new timeline after the last date in a timeline passes.

static let never: TimelineReloadPolicy

A policy that specifies that the app prompts WidgetKit when a new timeline is available.

