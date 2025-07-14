

- SwiftUI
- NavigationSplitView
-  init(columnVisibility:sidebar:detail:) 

Initializer

# init(columnVisibility:sidebar:detail:)

Creates a two-column navigation split view that enables programmatic control of the sidebar’s visibility.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    columnVisibility: Binding,
    @ViewBuilder sidebar: () -> Sidebar,
    @ViewBuilder detail: () -> Detail
) where Content == EmptyView
```

## Parameters 

`columnVisibility`  

A Binding to state that controls the visibility of the leading column.

`sidebar`  

The view to show in the leading column.

`detail`  

The view to show in the detail area.

## See Also

### Hiding columns in a navigation split view

init(columnVisibility: Binding&lt;NavigationSplitViewVisibility>, sidebar: () -> Sidebar, content: () -> Content, detail: () -> Detail)

Creates a three-column navigation split view that enables programmatic control of leading columns’ visibility.

