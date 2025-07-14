

- SwiftUI
- MenuBarExtra
-  init(content:label:) 

Initializer

# init(content:label:)

Creates a menu bar extra that will be displayed in the system menu bar, and defines the primary scene of an `App`.

macOS 13.0+

``` source
init(
    @ViewBuilder content: () -> Content,
    @ViewBuilder label: () -> Label
)
```

## Parameters 

`content`  

A `View` to display when the user selects the item.

`label`  

A `View` to use as the label in the system menu bar.

## Discussion

When this item is removed from the system menu bar by the user, the application will be automatically quit. As such, it should not be used in conjunction with other scene types in your `App`.

## See Also

### Creating a menu bar extra

init(_:content:)

Creates a menu bar extra with a key for a localized string to use as the label. The extra defines the primary scene of an `App`.

init(_:isInserted:content:)

Creates a menu bar extra with a key for a localized string to use as the label. The item will be displayed in the system menu bar when the specified binding is set to `true`. If the user removes the item from the menu bar, the binding will be set to `false`.

init(isInserted: Binding&lt;Bool>, content: () -> Content, label: () -> Label)

Creates a menu bar extra. The item will be displayed in the system menu bar when the specified binding is set to `true`. If the user removes the item from the menu bar, the binding will be set to `false`.

