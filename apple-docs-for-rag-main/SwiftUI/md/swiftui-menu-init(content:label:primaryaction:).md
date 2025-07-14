

- SwiftUI
- Menu
-  init(content:label:primaryAction:) 

Initializer

# init(content:label:primaryAction:)

Creates a menu with a custom primary action and custom label.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
nonisolated
init(
    @ViewBuilder content: () -> Content,
    @ViewBuilder label: () -> Label,
    primaryAction: @escaping () -> Void
)
```

Available when `Label` conforms to `View` and `Content` conforms to `View`.

## Parameters 

`content`  

A group of menu items.

`label`  

A view describing the content of the menu.

`primaryAction`  

The action to perform on primary interaction with the menu.

## See Also

### Creating a menu with a primary action

init(_:content:primaryAction:)

Creates a menu with a custom primary action that generates its label from a localized string key.

init(LocalizedStringKey, image: ImageResource, content: () -> Content, primaryAction: () -> Void)

Creates a menu with a custom primary action that generates its label from a localized string key.

init(LocalizedStringKey, systemImage: String, content: () -> Content, primaryAction: () -> Void)

Creates a menu with a custom primary action that generates its label from a localized string key and system image.

