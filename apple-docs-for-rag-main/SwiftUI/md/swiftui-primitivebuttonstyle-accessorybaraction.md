

- SwiftUI
- PrimitiveButtonStyle
-  accessoryBarAction 

Type Property

# accessoryBarAction

A button style that you use for extra actions in an accessory toolbar.

macOS 14.0+

``` source
@MainActor @preconcurrency
static var accessoryBarAction: AccessoryBarActionButtonStyle { get }
```

Available when `Self` is `AccessoryBarActionButtonStyle`.

## Discussion

Use this style for buttons that perform extra actions relative to the accessory toolbar’s main functions, like adding or editing filters. This style also affects other view types that you apply a button style to, like Toggle, Picker, and Menu instances.

## See Also

### Getting built-in button styles

static var automatic: DefaultButtonStyle

The default button style, based on the button’s context.

static var accessoryBar: AccessoryBarButtonStyle

A button style that is typically used in the context of an accessory toolbar (sometimes refererred to as a “scope bar”), for buttons that narrow the focus of a search or other operation.

static var bordered: BorderedButtonStyle

A button style that applies standard border artwork based on the button’s context.

static var borderedProminent: BorderedProminentButtonStyle

A button style that applies standard border prominent artwork based on the button’s context.

static var borderless: BorderlessButtonStyle

A button style that doesn’t apply a border.

static var card: CardButtonStyle

A button style that doesn’t pad the content, and applies a motion effect when a button has focus.

static var link: LinkButtonStyle

A button style for buttons that emulate links.

static var plain: PlainButtonStyle

A button style that doesn’t style or decorate its content while idle, but may apply a visual effect to indicate the pressed, focused, or enabled state of the button.

