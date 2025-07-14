

- SwiftUI
- DatePickerStyle
-  graphical 

Type Property

# graphical

A date picker style that displays an interactive calendar or clock.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+visionOS 1.0+

``` source
@MainActor @preconcurrency
static var graphical: GraphicalDatePickerStyle { get }
```

Available when `Self` is `GraphicalDatePickerStyle`.

## Discussion

This style is useful when you want to allow browsing through days in a calendar, or when the look of a clock face is appropriate.

## See Also

### Getting built-in date picker styles

static var automatic: DefaultDatePickerStyle

The default style for date pickers.

static var compact: CompactDatePickerStyle

A date picker style that displays the components in a compact, textual format.

static var field: FieldDatePickerStyle

A date picker style that displays the components in an editable field.

static var stepperField: StepperFieldDatePickerStyle

A system style that displays the components in an editable field, with adjoining stepper that can increment/decrement the selected component.

static var wheel: WheelDatePickerStyle

A date picker style that displays each component as columns in a scrollable wheel.

