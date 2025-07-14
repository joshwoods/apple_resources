

- SwiftUI
- PrimitiveButtonStyle
-  accessoryBar 

Type Property

# accessoryBar

A button style that is typically used in the context of an accessory toolbar (sometimes refererred to as a “scope bar”), for buttons that narrow the focus of a search or other operation.

macOS 14.0+

``` source
@MainActor @preconcurrency
static var accessoryBar: AccessoryBarButtonStyle { get }
```

Available when `Self` is `AccessoryBarButtonStyle`.

## Discussion

This is the default button style for views in accessory toolbars, created with `ToolbarItemPlacement.init(id:_)`, and for searchable scopes.

This style will also affect button style `Toggle`s, as well as button style `Picker`s and `Menu`s.

```
HStack(alignment: .firstTextBaseline) {
    Button("Button") {}

    Toggle("Toggle", isOn: $isToggleOn)
        .toggleStyle(.button)

    Picker("Picker", selection: $selection) {
        Text("Option 1").tag(0)
        Text("Option 2").tag(1)
    }

    Picker("Inline Picker", selection: $selection) {
        Text("Option 1").tag(0)
        Text("Option 2").tag(1)
    }
    .pickerStyle(.inline)

    Menu("Menu") {
        Button("Item") {}
    }
}
.buttonStyle(.accessoryBar)
```

## See Also

### Getting built-in button styles

static var automatic: DefaultButtonStyle

The default button style, based on the button’s context.

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

