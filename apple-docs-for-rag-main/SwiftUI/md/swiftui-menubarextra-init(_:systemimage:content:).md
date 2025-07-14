

- SwiftUI
- MenuBarExtra
-  init(\_:systemImage:content:) 

Initializer

# init(\_:systemImage:content:)

Creates a menu bar extra with a system image to use as the items label. The provided title will be used by the accessibility system.

macOS 13.0+

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    systemImage: String,
    @ViewBuilder content: () -> Content
)
```

Available when `Label` is `Label` and `Content` conforms to `View`.

Show all declarations

## Parameters 

`titleKey`  

The localized string key to use for the accessibility label of the item.

`systemImage`  

The name of a system image to use as the label.

`content`  

A `View` to display when the user selects the item.

## Discussion

The item defines the primary scene of an `App`.

When this item is removed from the system menu bar by the user, the application will be automatically quit. As such, it should not be used in conjunction with other scene types in your `App`.

## See Also

### Creating a menu bar extra with an image

init(_:image:content:)

Creates a menu bar extra with an image to use as the items label. The provided title will be used by the accessibility system.

init(_:image:isInserted:content:)

Creates a menu bar extra with an image to use as the items label. The provided title will be used by the accessibility system.

init(_:systemImage:isInserted:content:)

Creates a menu bar extra with a system image to use as the items label. The provided title will be used by the accessibility system.

