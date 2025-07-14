

- SwiftUI
- ToolbarItem
-  init(id:placement:showsByDefault:content:) Deprecated

Initializer

# init(id:placement:showsByDefault:content:)

Creates a toolbar item with the specified placement and content, which allows for user customization.

iOS 14.0–18.4DeprecatediPadOS 14.0–18.4DeprecatedMac Catalyst 14.0–18.4DeprecatedmacOS 11.0–15.4DeprecatedtvOS 14.0–18.4DeprecatedvisionOS 1.0+watchOS 7.0–11.4Deprecated

``` source
nonisolated
init(
    id: String,
    placement: ToolbarItemPlacement = .automatic,
    showsByDefault: Bool,
    @ViewBuilder content: () -> Content
)
```

Available when `ID` is `String` and `Content` conforms to `View`.

Deprecated

Use the CustomizableToolbarContent/defaultCustomization(\_:options) modifier with a value of .hidden

## Parameters 

`id`  

A unique identifier for this item.

`placement`  

Which section of the toolbar the item should be placed in.

`showsByDefault`  

Whether the item appears by default in the toolbar, or only shows if the user explicitly adds it via customization.

`content`  

The content of the item.

## See Also

### Creating a toolbar item

init(placement: ToolbarItemPlacement, content: () -> Content)

Creates a toolbar item with the specified placement and content.

init(id: String, placement: ToolbarItemPlacement, content: () -> Content)

Creates a toolbar item with the specified placement and content, which allows for user customization.

