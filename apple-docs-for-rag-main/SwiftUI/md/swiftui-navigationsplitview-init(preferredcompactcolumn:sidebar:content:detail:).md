

- SwiftUI
- NavigationSplitView
-  init(preferredCompactColumn:sidebar:content:detail:) 

Initializer

# init(preferredCompactColumn:sidebar:content:detail:)

Creates a three-column navigation split view that enables programmatic control over which column appears on top when the view collapses into a single column in narrow sizes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
init(
    preferredCompactColumn: Binding,
    @ViewBuilder sidebar: () -> Sidebar,
    @ViewBuilder content: () -> Content,
    @ViewBuilder detail: () -> Detail
)
```

Available when `Sidebar` conforms to `View`, `Content` conforms to `View`, and `Detail` conforms to `View`.

## Parameters 

`preferredCompactColumn`  

A Binding to state that controls which column appears on top when the view collapses.

`sidebar`  

The view to show in the leading column.

`content`  

The view to show in the middle column.

`detail`  

The view to show in the detail area.

## See Also

### Specifying a preferred compact column

init(preferredCompactColumn: Binding&lt;NavigationSplitViewColumn>, sidebar: () -> Sidebar, detail: () -> Detail)

Creates a two-column navigation split view that enables programmatic control over which column appears on top when the view collapses into a single column in narrow sizes.

