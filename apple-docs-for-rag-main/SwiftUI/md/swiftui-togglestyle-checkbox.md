

- SwiftUI
- ToggleStyle
-  checkbox 

Type Property

# checkbox

A toggle style that displays a checkbox followed by its label.

macOS 10.15+

``` source
@MainActor @preconcurrency
static var checkbox: CheckboxToggleStyle { get }
```

Available when `Self` is `CheckboxToggleStyle`.

## Discussion

Apply this style to a Toggle or to a view hierarchy that contains toggles using the toggleStyle(_:) modifier:

```
Toggle("Close windows when quitting an app", isOn: $doesClose)
    .toggleStyle(.checkbox)
```

The style produces a label that describes the purpose of the toggle and a checkbox that shows the toggle’s state. To change the toggle’s state, the user clicks the checkbox or its label:

The style aligns the trailing edge of the checkbox with the leading edge of the label, and takes as much horizontal space as it needs to fit the label, up to the amount offered by the toggle’s parent view.

This is the default style in macOS in most contexts when you don’t set a style, or when you apply the automatic style. A Form is a convenient way to present a collection of checkboxes with proper spacing and alignment. For guidance on using checkboxes in your user interface, see Toggles in the Human Interface Guidelines.

## See Also

### Getting built-in toggle styles

static var automatic: DefaultToggleStyle

The default toggle style.

static var button: ButtonToggleStyle

A toggle style that displays as a button with its label as the title.

static var `switch`: SwitchToggleStyle

A toggle style that displays a leading label and a trailing switch.

