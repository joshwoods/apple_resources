

- SwiftUI
- Tab
-  init(\_:systemImage:role:content:) 

Initializer

# init(\_:systemImage:role:content:)

Creates a new tab that you can use in a tab view using a system image for the tab item’s image, and a localized string key label.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    _ titleKey: LocalizedStringKey,
    systemImage: String,
    role: TabRole?,
    @ViewBuilder content: () -> Content
) where Label == DefaultTabLabel
```

Available when `Value` is `Never`, `Content` conforms to `View`, and `Label` conforms to `View`.

Show all declarations

## Parameters 

`titleKey`  

The localized string key label for the tab’s tab item.

`role`  

The role defining the semantic purpose of the tab.

`content`  

The view content of the tab.

## See Also

### Creating a tab with system symbol

init(_:systemImage:content:)

Creates a new tab that you can use in a tab view using a system image for the tab item’s image, and a localized string key label.

init(_:systemImage:value:content:)

Creates a tab that the tab view presents when the tab view’s selection matches the tab’s value using a system image for the tab’s tab item image, with a localized string key label.

init(_:systemImage:value:role:content:)

Creates a tab that the tab view presents when the tab view’s selection matches the tab’s value using a system image for the tab’s tab item image, with a localized string key label.

