

- SwiftUI
- ToolbarItemGroup
-  init(placement:content:label:) 

Initializer

# init(placement:content:label:)

Creates a toolbar item group with the specified placement, content, and a label describing that content.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    placement: ToolbarItemPlacement = .automatic,
    @ViewBuilder content: () -> C,
    @ViewBuilder label: () -> L
) where Content == LabeledToolbarItemGroupContent, C : View, L : View
```

Available when `Content` conforms to `View`.

## Parameters 

`placement`  

Which section of the toolbar the item should be placed in.

`content`  

The content of the item.

`label`  

The label describing the content of the item.

## Discussion

A toolbar item group provided a label wraps its content within a ControlGroup which allows the content to collapse down into a menu that presents its content based on available space.

## See Also

### Creating a toolbar item group

init(placement: ToolbarItemPlacement, content: () -> Content)

Creates a toolbar item group with a specified placement and content.

