

- SwiftUI
- NavigationSplitView
-  init(sidebar:detail:) 

Initializer

# init(sidebar:detail:)

Creates a two-column navigation split view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    @ViewBuilder sidebar: () -> Sidebar,
    @ViewBuilder detail: () -> Detail
) where Content == EmptyView
```

## Parameters 

`sidebar`  

The view to show in the leading column.

`detail`  

The view to show in the detail area.

## Mentioned in 

Migrating to new navigation types

## See Also

### Creating a navigation split view

init(sidebar: () -> Sidebar, content: () -> Content, detail: () -> Detail)

Creates a three-column navigation split view.

