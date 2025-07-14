

- SwiftUI
- Tab
-  init(value:content:) 

Initializer

# init(value:content:)

Creates a new tab that you can use in a tab view, with an empty label.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
init(
    value: Value,
    @ViewBuilder content: () -> Content
) where Label == EmptyView
```

Available when `Value` conforms to `Hashable`, `Content` conforms to `View`, and `Label` conforms to `View`.

Show all declarations

## Parameters 

`value`  

The `selection` value which selects this tab.

`content`  

The view content of the tab.

## See Also

### Creating a tab

init(content: () -> Content)

Creates a new tab that you can use in a tab view, with an empty label.

init(role: TabRole?, content: () -> Content)

Creates a new tab that you can use in a tab view, with an empty label.

init(value:role:content:)

Creates a new tab with a label inferred from the role.

