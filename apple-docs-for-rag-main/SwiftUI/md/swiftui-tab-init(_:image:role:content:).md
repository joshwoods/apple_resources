

- SwiftUI
- Tab
-  init(\_:image:role:content:) 

Initializer

# init(\_:image:role:content:)

Creates a new tab that you can use in a tab view, with a localized string key label.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    _ titleKey: LocalizedStringKey,
    image: String,
    role: TabRole?,
    @ViewBuilder content: () -> Content
) where Label == DefaultTabLabel
```

Available when `Value` is `Never`, `Content` conforms to `View`, and `Label` conforms to `View`.

Show all declarations

## Parameters 

`titleKey`  

The localized string key label for the tab’s tab item.

`image`  

The image for the tab’s tab item.

`role`  

The role defining the semantic purpose of the tab.

`content`  

The view content of the tab.

## See Also

### Creating a tab with image

init(_:image:content:)

Creates a new tab that you can use in a tab view, with a localized string key label.

init(_:image:value:content:)

Creates a tab that the tab view presents when the tab view’s selection matches the tab’s value, with a localized string key label.

init(_:image:value:role:content:)

Creates a tab that the tab view presents when the tab view’s selection matches the tab’s value, with a localized string key label.

