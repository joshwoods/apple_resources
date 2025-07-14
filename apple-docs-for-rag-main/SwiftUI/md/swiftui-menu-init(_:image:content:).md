

- SwiftUI
- Menu
-  init(\_:image:content:) 

Initializer

# init(\_:image:content:)

Creates a menu that generates its label from a localized string key and image resource.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    image: ImageResource,
    @ViewBuilder content: () -> Content
)
```

Available when `Label` is `Label` and `Content` conforms to `View`.

Show all declarations

## Parameters 

`titleKey`  

The key for the link’s localized title, which describes the contents of the menu.

`image`  

The name of the image resource to lookup.

`content`  

A group of menu items.

## See Also

### Creating a menu from content

init(_:content:)

Creates a menu that generates its label from a localized string key.

init(content: () -> Content, label: () -> Label)

Creates a menu with a custom label.

init(_:systemImage:content:)

Creates a menu that generates its label from a localized string key and system image.

