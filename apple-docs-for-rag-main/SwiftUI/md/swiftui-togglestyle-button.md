

- SwiftUI
- ToggleStyle
-  button 

Type Property

# button

A toggle style that displays as a button with its label as the title.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
static var button: ButtonToggleStyle { get }
```

Available when `Self` is `ButtonToggleStyle`.

## Discussion

Apply this style to a Toggle or to a view hierarchy that contains toggles using the toggleStyle(_:) modifier:

```
Toggle(isOn: $isFlagged) {
    Label("Flag", systemImage: "flag.fill")
}
.toggleStyle(.button)
```

The style produces a button with a label that describes the purpose of the toggle. The user taps or clicks the button to change the toggle’s state. The button indicates the `on` state by filling in the background with its tint color. You can change the tint color using the tint(_:) modifier. SwiftUI uses this style as the default for toggles that appear in a toolbar.

The following table shows the toggle in both the `off` and `on` states, respectively:

| Platform | Appearance |
|----|----|
| iOS, iPadOS |  |
| macOS |  |

A Label instance is a good choice for a button toggle’s label. Based on the context, SwiftUI decides whether to display both the title and icon, as in the example above, or just the icon, like when the toggle appears in a toolbar. You can also control the label’s style by adding a labelStyle(_:) modifier. In any case, SwiftUI always uses the title to identify the control using VoiceOver.

## See Also

### Getting built-in toggle styles

static var automatic: DefaultToggleStyle

The default toggle style.

static var checkbox: CheckboxToggleStyle

A toggle style that displays a checkbox followed by its label.

static var `switch`: SwitchToggleStyle

A toggle style that displays a leading label and a trailing switch.

