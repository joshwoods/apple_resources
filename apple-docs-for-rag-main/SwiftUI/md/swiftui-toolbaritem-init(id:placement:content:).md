

- SwiftUI
- ToolbarItem
-  init(id:placement:content:) 

Initializer

# init(id:placement:content:)

Creates a toolbar item with the specified placement and content, which allows for user customization.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
init(
    id: String,
    placement: ToolbarItemPlacement = .automatic,
    @ViewBuilder content: () -> Content
)
```

Available when `ID` is `String` and `Content` conforms to `View`.

## Parameters 

`id`  

A unique identifier for this item.

`placement`  

Which section of the toolbar the item should be placed in.

`content`  

The content of the item.

## See Also

### Creating a toolbar item

init(placement: ToolbarItemPlacement, content: () -> Content)

Creates a toolbar item with the specified placement and content.

init(id: String, placement: ToolbarItemPlacement, showsByDefault: Bool, content: () -> Content)

Creates a toolbar item with the specified placement and content, which allows for user customization.

Deprecated

