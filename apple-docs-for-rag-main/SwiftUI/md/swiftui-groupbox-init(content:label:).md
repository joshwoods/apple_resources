

- SwiftUI
- GroupBox
-  init(content:label:) 

Initializer

# init(content:label:)

Creates a group box with the provided label and view content.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+visionOS 1.0+

``` source
init(
    @ViewBuilder content: () -> Content,
    @ViewBuilder label: () -> Label
)
```

## Parameters 

`content`  

A ViewBuilder that produces the content for the group box.

`label`  

A ViewBuilder that produces a label for the group box.

## See Also

### Creating a group box

init(content: () -> Content)

Creates an unlabeled group box with the provided view content.

init(_:content:)

Creates a group box with the provided view content and title.

