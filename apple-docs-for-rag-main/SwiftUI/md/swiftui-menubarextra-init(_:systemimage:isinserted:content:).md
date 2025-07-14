

- SwiftUI
- MenuBarExtra
-  init(\_:systemImage:isInserted:content:) 

Initializer

# init(\_:systemImage:isInserted:content:)

Creates a menu bar extra with a system image to use as the items label. The provided title will be used by the accessibility system.

macOS 13.0+

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    systemImage: String,
    isInserted: Binding,
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

`isInserted`  

Whether the item is inserted in the menu bar. The item may or may not be visible, depending on the number of items present.

`content`  

A `View` to display when the user selects the item.

## Discussion

The item will be displayed in the system menu bar when the specified binding is set to `true`. If the user removes the item from the menu bar, the binding will be set to `false`.

## See Also

### Creating a menu bar extra with an image

init(_:image:content:)

Creates a menu bar extra with an image to use as the items label. The provided title will be used by the accessibility system.

init(_:image:isInserted:content:)

Creates a menu bar extra with an image to use as the items label. The provided title will be used by the accessibility system.

init(_:systemImage:content:)

Creates a menu bar extra with a system image to use as the items label. The provided title will be used by the accessibility system.

