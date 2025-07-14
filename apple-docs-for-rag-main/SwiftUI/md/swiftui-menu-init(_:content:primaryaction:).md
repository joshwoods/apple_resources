

- SwiftUI
- Menu
-  init(\_:content:primaryAction:) 

Initializer

# init(\_:content:primaryAction:)

Creates a menu with a custom primary action that generates its label from a localized string key.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    @ViewBuilder content: () -> Content,
    primaryAction: @escaping () -> Void
) where Label == Text
```

Available when `Label` conforms to `View` and `Content` conforms to `View`.

Show all declarations

## Parameters 

`titleKey`  

The key for the link’s localized title, which describes the contents of the menu.

`content`  

A group of menu items.

`primaryAction`  

The action to perform on primary interaction with the menu.

## See Also

### Creating a menu with a primary action

init(content: () -> Content, label: () -> Label, primaryAction: () -> Void)

Creates a menu with a custom primary action and custom label.

init(LocalizedStringKey, image: ImageResource, content: () -> Content, primaryAction: () -> Void)

Creates a menu with a custom primary action that generates its label from a localized string key.

init(LocalizedStringKey, systemImage: String, content: () -> Content, primaryAction: () -> Void)

Creates a menu with a custom primary action that generates its label from a localized string key and system image.

