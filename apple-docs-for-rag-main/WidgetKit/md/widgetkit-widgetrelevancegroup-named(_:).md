

- WidgetKit
- WidgetRelevanceGroup
-  named(\_:) 

Type Method

# named(\_:)

Creates a group with the provided name. Widgets in the same group will not be suggested by the system simultaneously in contexts where both are visible. Named groups are namespaced to the containing app, and won’t be impacted by other apps.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+watchOS 11.0+

``` source
static func named(_ name: String) -> WidgetRelevanceGroup
```

