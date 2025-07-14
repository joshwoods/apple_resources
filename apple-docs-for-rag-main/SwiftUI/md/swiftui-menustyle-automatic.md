

- SwiftUI
- MenuStyle
-  automatic 

Type Property

# automatic

The default menu style, based on the menu’s context.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
static var automatic: DefaultMenuStyle { get }
```

Available when `Self` is `DefaultMenuStyle`.

## Discussion

The default menu style can vary by platform. By default, macOS uses the bordered button style.

If you create a menu inside a container, the style resolves to the recommended style for menus inside that container for that specific platform. For example, a menu nested within another menu will resolve to a submenu:

```
Menu("Edit") {
    Menu("Arrange") {
        Button("Bring to Front", action: moveSelectionToFront)
        Button("Send to Back", action: moveSelectionToBack)
    }
    Button("Delete", action: deleteSelection)
}
```

You can override a menu’s style. To apply the default style to a menu, or to a view that contains a menu, use the menuStyle(_:) modifier.

## See Also

### Getting built-in menu styles

static var button: ButtonMenuStyle

A menu style that displays a button that toggles the display of the menu’s contents when pressed.

static var borderedButton: BorderedButtonMenuStyle

A menu style that displays a bordered button that toggles the display of the menu’s contents when pressed.

Deprecated

static var borderlessButton: BorderlessButtonMenuStyle

A menu style that displays a borderless button that toggles the display of the menu’s contents when pressed.

Deprecated

