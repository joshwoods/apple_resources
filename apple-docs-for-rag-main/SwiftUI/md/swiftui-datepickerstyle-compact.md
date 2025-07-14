

- SwiftUI
- DatePickerStyle
-  compact 

Type Property

# compact

A date picker style that displays the components in a compact, textual format.

iOS 14.0+iPadOS 14.0+Mac Catalyst 13.4+macOS 10.15.4+visionOS 1.0+

``` source
@MainActor @preconcurrency
static var compact: CompactDatePickerStyle { get }
```

Available when `Self` is `CompactDatePickerStyle`.

## Discussion

Use this style when space is constrained and users expect to make specific date and time selections. Some variants may include rich editing controls in a pop up.

## See Also

### Getting built-in date picker styles

static var automatic: DefaultDatePickerStyle

The default style for date pickers.

static var field: FieldDatePickerStyle

A date picker style that displays the components in an editable field.

static var graphical: GraphicalDatePickerStyle

A date picker style that displays an interactive calendar or clock.

static var stepperField: StepperFieldDatePickerStyle

A system style that displays the components in an editable field, with adjoining stepper that can increment/decrement the selected component.

static var wheel: WheelDatePickerStyle

A date picker style that displays each component as columns in a scrollable wheel.

