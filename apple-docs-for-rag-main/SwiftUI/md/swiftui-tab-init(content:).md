

- SwiftUI
- Tab
-  init(content:) 

Initializer

# init(content:)

Creates a new tab that you can use in a tab view, with an empty label.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(@ViewBuilder content: () -> Content) where Label == EmptyView
```

Available when `Value` is `Never`, `Content` conforms to `View`, and `Label` conforms to `View`.

## Parameters 

`content`  

The view content of the tab.

## See Also

### Creating a tab

init(value:content:)

Creates a new tab that you can use in a tab view, with an empty label.

init(role: TabRole?, content: () -> Content)

Creates a new tab that you can use in a tab view, with an empty label.

init(value:role:content:)

Creates a new tab with a label inferred from the role.

