

- SwiftUI
- Menu
-  init(\_:content:) 

Initializer

# init(\_:content:)

Creates a menu that generates its label from a localized string key.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 17.0+visionOS 1.0+

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    @ViewBuilder content: () -> Content
) where Label == Text
```

Available when `Label` conforms to `View` and `Content` conforms to `View`.

Show all declarations

## Parameters 

`titleKey`  

The key for the link’s localized title, which describes the contents of the menu.

`content`  

A group of menu items.

## See Also

### Creating a menu from content

init(content: () -> Content, label: () -> Label)

Creates a menu with a custom label.

init(_:image:content:)

Creates a menu that generates its label from a localized string key and image resource.

init(_:systemImage:content:)

Creates a menu that generates its label from a localized string key and system image.

