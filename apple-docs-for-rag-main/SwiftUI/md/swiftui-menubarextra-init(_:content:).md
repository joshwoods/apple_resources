

- SwiftUI
- MenuBarExtra
-  init(\_:content:) 

Initializer

# init(\_:content:)

Creates a menu bar extra with a key for a localized string to use as the label. The extra defines the primary scene of an `App`.

macOS 13.0+

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    @ViewBuilder content: () -> Content
)
```

Available when `Label` is `Text` and `Content` conforms to `View`.

Show all declarations

## Parameters 

`titleKey`  

The title key to use for the label of the item.

`content`  

A `View` to display when the user selects the item.

## Discussion

When this item is removed from the system menu bar by the user, the application will be automatically quit. As such, it should not be used in conjunction with other scene types in your `App`.

## See Also

### Creating a menu bar extra

init(content: () -> Content, label: () -> Label)

Creates a menu bar extra that will be displayed in the system menu bar, and defines the primary scene of an `App`.

init(_:isInserted:content:)

Creates a menu bar extra with a key for a localized string to use as the label. The item will be displayed in the system menu bar when the specified binding is set to `true`. If the user removes the item from the menu bar, the binding will be set to `false`.

init(isInserted: Binding&lt;Bool>, content: () -> Content, label: () -> Label)

Creates a menu bar extra. The item will be displayed in the system menu bar when the specified binding is set to `true`. If the user removes the item from the menu bar, the binding will be set to `false`.

