

- SwiftUI
- ToolbarItem
-  init(placement:content:) 

Initializer

# init(placement:content:)

Creates a toolbar item with the specified placement and content.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
init(
    placement: ToolbarItemPlacement = .automatic,
    @ViewBuilder content: () -> Content
)
```

Available when `ID` is `()` and `Content` conforms to `View`.

## Parameters 

`placement`  

Which section of the toolbar the item should be placed in.

`content`  

The content of the item.

## See Also

### Creating a toolbar item

init(id: String, placement: ToolbarItemPlacement, content: () -> Content)

Creates a toolbar item with the specified placement and content, which allows for user customization.

init(id: String, placement: ToolbarItemPlacement, showsByDefault: Bool, content: () -> Content)

Creates a toolbar item with the specified placement and content, which allows for user customization.

Deprecated

