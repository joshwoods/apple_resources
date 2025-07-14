

- SwiftUI
- ToggleStyle
-  switch 

Type Property

# switch

A toggle style that displays a leading label and a trailing switch.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 18.0+visionOS 1.0+watchOS 6.0+

``` source
@MainActor @preconcurrency
static var `switch`: SwitchToggleStyle { get }
```

Available when `Self` is `SwitchToggleStyle`.

## Discussion

Apply this style to a Toggle or to a view hierarchy that contains toggles using the toggleStyle(_:) modifier:

```
Toggle("Enhance Sound", isOn: $isEnhanced)
    .toggleStyle(.switch)
```

The style produces a label that describes the purpose of the toggle and a switch that shows the toggle’s state. The user taps or clicks the switch to change the toggle’s state. The default appearance is similar across platforms, although the way you use switches in your user interface varies a little, as described in Toggles in the Human Interface Guidelines.

- iOS
- macOS
- watchOS
- tvOS

In iOS, iPadOS, watchOS, and tvOS, the label and switch fill as much horizontal space as the toggle’s parent offers by aligning the label’s leading edge and the switch’s trailing edge with the containing view’s respective leading and trailing edges. In macOS, the style uses a minimum of horizontal space by aligning the trailing edge of the label with the leading edge of the switch. SwiftUI helps you to manage the spacing and alignment when this style appears in a Form.

SwiftUI uses this style as the default for iOS, iPadOS, watchOS, and tvOS in most contexts when you don’t set a style, or when you apply the automatic style.

## See Also

### Getting built-in toggle styles

static var automatic: DefaultToggleStyle

The default toggle style.

static var button: ButtonToggleStyle

A toggle style that displays as a button with its label as the title.

static var checkbox: CheckboxToggleStyle

A toggle style that displays a checkbox followed by its label.

