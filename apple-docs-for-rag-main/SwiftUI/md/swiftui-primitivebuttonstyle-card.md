

- SwiftUI
- PrimitiveButtonStyle
-  card 

Type Property

# card

A button style that doesn’t pad the content, and applies a motion effect when a button has focus.

tvOS 14.0+

``` source
@MainActor @preconcurrency
static var card: CardButtonStyle { get }
```

Available when `Self` is `CardButtonStyle`.

## Discussion

This style doesn’t apply padding to its contents, so images, text, and other content display edge-to-edge. A button with this style appears partially translucent. When the user focuses on a card button, the button animates up to a raised position with more opacity. This style also applies the standard background colors for unfocused and focused states in both light and dark mode.

To apply this style to a button, or to a view that contains buttons, use the buttonStyle(_:) modifier.

## See Also

### Getting built-in button styles

static var automatic: DefaultButtonStyle

The default button style, based on the button’s context.

static var accessoryBar: AccessoryBarButtonStyle

A button style that is typically used in the context of an accessory toolbar (sometimes refererred to as a “scope bar”), for buttons that narrow the focus of a search or other operation.

static var accessoryBarAction: AccessoryBarActionButtonStyle

A button style that you use for extra actions in an accessory toolbar.

static var bordered: BorderedButtonStyle

A button style that applies standard border artwork based on the button’s context.

static var borderedProminent: BorderedProminentButtonStyle

A button style that applies standard border prominent artwork based on the button’s context.

static var borderless: BorderlessButtonStyle

A button style that doesn’t apply a border.

static var link: LinkButtonStyle

A button style for buttons that emulate links.

static var plain: PlainButtonStyle

A button style that doesn’t style or decorate its content while idle, but may apply a visual effect to indicate the pressed, focused, or enabled state of the button.

