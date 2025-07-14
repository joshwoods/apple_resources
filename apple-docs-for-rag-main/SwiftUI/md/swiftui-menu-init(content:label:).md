

- SwiftUI
- Menu
-  init(content:label:) 

Initializer

# init(content:label:)

Creates a menu with a custom label.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 17.0+visionOS 1.0+

``` source
nonisolated
init(
    @ViewBuilder content: () -> Content,
    @ViewBuilder label: () -> Label
)
```

Available when `Label` conforms to `View` and `Content` conforms to `View`.

## Parameters 

`content`  

A group of menu items.

`label`  

A view describing the content of the menu.

## See Also

### Creating a menu from content

init(_:content:)

Creates a menu that generates its label from a localized string key.

init(_:image:content:)

Creates a menu that generates its label from a localized string key and image resource.

init(_:systemImage:content:)

Creates a menu that generates its label from a localized string key and system image.

