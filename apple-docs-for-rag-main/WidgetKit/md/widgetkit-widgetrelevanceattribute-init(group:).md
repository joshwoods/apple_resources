

- WidgetKit
- WidgetRelevanceAttribute
-  init(group:) 

Initializer

# init(group:)

Associates the widget kind with a group. When multiple widgets are in the same group, the system will only suggest one member of the group simultaneously. Widgets in the same group are interpreted to contain redundant information, and therefore should not be presented together.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+watchOS 11.0+

``` source
init(group: WidgetRelevanceGroup)
```

Available when `Configuration` is `()`.

## Parameters 

`group`  

The group to associate the widget with

## Discussion

Multiple groups can be associated with the same widget by providing multiple `WidgetRelevanceAttribute` instances with different groups.

