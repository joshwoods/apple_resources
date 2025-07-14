

- SwiftUI
- MenuStyle
-  borderlessButton Deprecated

Type Property

# borderlessButton

A menu style that displays a borderless button that toggles the display of the menu’s contents when pressed.

iOS 14.0–18.4DeprecatediPadOS 14.0–18.4DeprecatedMac Catalyst 14.0–18.4DeprecatedmacOS 11.0–15.4DeprecatedtvOS 17.0–18.4DeprecatedvisionOS 1.0–2.4Deprecated

``` source
@MainActor @preconcurrency
static var borderlessButton: BorderlessButtonMenuStyle { get }
```

Available when `Self` is `BorderlessButtonMenuStyle`.

Deprecated

Use menuStyle(_:) with button and buttonStyle(_:) with borderless.

## Discussion

On macOS, the button optionally displays an arrow indicating that it presents a menu.

Pressing and then dragging into the contents triggers the chosen action on release.

## See Also

### Getting built-in menu styles

static var automatic: DefaultMenuStyle

The default menu style, based on the menu’s context.

static var button: ButtonMenuStyle

A menu style that displays a button that toggles the display of the menu’s contents when pressed.

static var borderedButton: BorderedButtonMenuStyle

A menu style that displays a bordered button that toggles the display of the menu’s contents when pressed.

Deprecated

