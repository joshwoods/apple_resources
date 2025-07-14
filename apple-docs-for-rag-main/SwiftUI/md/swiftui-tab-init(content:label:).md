

- SwiftUI
- Tab
-  init(content:label:) 

Initializer

# init(content:label:)

Creates a new tab with a label that you can use in a tab view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    @ViewBuilder content: () -> Content,
    @ViewBuilder label: () -> Label
)
```

Available when `Value` is `Never`, `Content` conforms to `View`, and `Label` conforms to `View`.

## Parameters 

`content`  

The view content of the tab.

`label`  

The label for the tab’s tab item.

