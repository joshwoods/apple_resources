

- SwiftUI
- PrimitiveButtonStyle
-  automatic 

Type Property

# automatic

The default button style, based on the button’s context.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@MainActor @preconcurrency
static var automatic: DefaultButtonStyle { get }
```

Available when `Self` is `DefaultButtonStyle`.

## Discussion

If you create a button directly on a blank canvas, the style varies by platform. iOS uses the borderless button style by default, whereas macOS, tvOS, and watchOS use the bordered button style.

If you create a button inside a container, like a List, the style resolves to the recommended style for buttons inside that container for that specific platform.

You can override a button’s style. To apply the default style to a button, or to a view that contains buttons, use the buttonStyle(_:) modifier.

## See Also

### Getting built-in button styles

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

static var card: CardButtonStyle

A button style that doesn’t pad the content, and applies a motion effect when a button has focus.

static var link: LinkButtonStyle

A button style for buttons that emulate links.

static var plain: PlainButtonStyle

A button style that doesn’t style or decorate its content while idle, but may apply a visual effect to indicate the pressed, focused, or enabled state of the button.

