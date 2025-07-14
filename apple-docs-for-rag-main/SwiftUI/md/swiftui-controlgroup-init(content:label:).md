

- SwiftUI
- ControlGroup
-  init(content:label:) 

Initializer

# init(content:label:)

Creates a new control group with the specified content and a label.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 17.0+visionOS 1.0+

``` source
nonisolated
init(
    @ViewBuilder content: () -> C,
    @ViewBuilder label: () -> L
) where Content == LabeledControlGroupContent, C : View, L : View
```

Available when `Content` conforms to `View`.

## Parameters 

`content`  

The content to display.

`label`  

A view that describes the purpose of the group.

## See Also

### Creating a control group

init(content: () -> Content)

Creates a new ControlGroup with the specified children

init(_:content:)

Creates a new control group with the specified content that generates its label from a string.

