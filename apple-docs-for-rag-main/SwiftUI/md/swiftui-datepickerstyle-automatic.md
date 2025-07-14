

- SwiftUI
- DatePickerStyle
-  automatic 

Type Property

# automatic

The default style for date pickers.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 10.0+

``` source
@MainActor @preconcurrency
static var automatic: DefaultDatePickerStyle { get }
```

Available when `Self` is `DefaultDatePickerStyle`.

## See Also

### Getting built-in date picker styles

static var compact: CompactDatePickerStyle

A date picker style that displays the components in a compact, textual format.

static var field: FieldDatePickerStyle

A date picker style that displays the components in an editable field.

static var graphical: GraphicalDatePickerStyle

A date picker style that displays an interactive calendar or clock.

static var stepperField: StepperFieldDatePickerStyle

A system style that displays the components in an editable field, with adjoining stepper that can increment/decrement the selected component.

static var wheel: WheelDatePickerStyle

A date picker style that displays each component as columns in a scrollable wheel.

