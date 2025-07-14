

- SwiftUI
- GroupBox
-  init(content:) 

Initializer

# init(content:)

Creates an unlabeled group box with the provided view content.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+visionOS 1.0+

``` source
nonisolated
init(@ViewBuilder content: () -> Content)
```

Available when `Label` is `EmptyView` and `Content` conforms to `View`.

## Parameters 

`content`  

A ViewBuilder that produces the content for the group box.

## See Also

### Creating a group box

init(content: () -> Content, label: () -> Label)

Creates a group box with the provided label and view content.

init(_:content:)

Creates a group box with the provided view content and title.

