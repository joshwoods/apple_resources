

- SwiftUI
- DatePickerStyle
-  stepperField 

Type Property

# stepperField

A system style that displays the components in an editable field, with adjoining stepper that can increment/decrement the selected component.

macOS 10.15+

``` source
@MainActor @preconcurrency
static var stepperField: StepperFieldDatePickerStyle { get }
```

Available when `Self` is `StepperFieldDatePickerStyle`.

## Discussion

This style is useful when space is constrained and users expect to make specific date and time selections.

## See Also

### Getting built-in date picker styles

static var automatic: DefaultDatePickerStyle

The default style for date pickers.

static var compact: CompactDatePickerStyle

A date picker style that displays the components in a compact, textual format.

static var field: FieldDatePickerStyle

A date picker style that displays the components in an editable field.

static var graphical: GraphicalDatePickerStyle

A date picker style that displays an interactive calendar or clock.

static var wheel: WheelDatePickerStyle

A date picker style that displays each component as columns in a scrollable wheel.

