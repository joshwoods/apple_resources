

- SwiftUI
- MenuStyle
-  borderedButton Deprecated

Type Property

# borderedButton

A menu style that displays a bordered button that toggles the display of the menu’s contents when pressed.

macOS 11.0–15.4Deprecated

``` source
@MainActor @preconcurrency
static var borderedButton: BorderedButtonMenuStyle { get }
```

Available when `Self` is `BorderedButtonMenuStyle`.

Deprecated

Use menuStyle(_:) with button and buttonStyle(_:) with bordered.

## Discussion

On macOS, the button displays an arrow indicating that it presents a menu.

Pressing and then dragging into the contents triggers the chosen action on release.

## See Also

### Getting built-in menu styles

static var automatic: DefaultMenuStyle

The default menu style, based on the menu’s context.

static var button: ButtonMenuStyle

A menu style that displays a button that toggles the display of the menu’s contents when pressed.

static var borderlessButton: BorderlessButtonMenuStyle

A menu style that displays a borderless button that toggles the display of the menu’s contents when pressed.

Deprecated

