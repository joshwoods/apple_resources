

- SwiftUI
-  DatePickerStyle 

Protocol

# DatePickerStyle

A type that specifies the appearance and interaction of all date pickers within a view hierarchy.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 10.0+

``` source
@MainActor @preconcurrency
protocol DatePickerStyle
```

## Overview

To configure the current date picker style for a view hierarchy, use the datePickerStyle(_:) modifier.

A type conforming to this protocol inherits `@preconcurrency @MainActor` isolation from the protocol if the conformance is included in the type’s base declaration:

```
struct MyCustomType: Transition {
    // `@preconcurrency @MainActor` isolation by default
}
```

Isolation to the main actor is the default, but it’s not required. Declare the conformance in an extension to opt out of main actor isolation:

```
extension MyCustomType: Transition {
    // `nonisolated` by default
}
```

## Topics

### Getting built-in date picker styles

static var automatic: DefaultDatePickerStyle

The default style for date pickers.

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

### Creating custom date picker styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Returns the appearance and interaction content for a `DatePicker`.

**Required**

struct DatePickerStyleConfiguration

The properties of a `DatePicker`.

typealias Configuration

A type alias for the properties of a `DatePicker`.

associatedtype Body : View

A view representing the appearance and interaction of a `DatePicker`.

**Required**

### Suporting types

struct DefaultDatePickerStyle

The default style for date pickers.

struct CompactDatePickerStyle

A date picker style that displays the components in a compact, textual format.

struct FieldDatePickerStyle

A date picker style that displays the components in an editable field.

struct GraphicalDatePickerStyle

A date picker style that displays an interactive calendar or clock.

struct StepperFieldDatePickerStyle

A system style that displays the components in an editable field, with adjoining stepper that can increment/decrement the selected component.

struct WheelDatePickerStyle

A date picker style that displays each component as columns in a scrollable wheel.

## Relationships

### Conforming Types

- CompactDatePickerStyle
- DefaultDatePickerStyle
- FieldDatePickerStyle
- GraphicalDatePickerStyle
- StepperFieldDatePickerStyle
- WheelDatePickerStyle

## See Also

### Styling pickers

func pickerStyle&lt;S>(S) -> some View

Sets the style for pickers within this view.

protocol PickerStyle

A type that specifies the appearance and interaction of all pickers within a view hierarchy.

func datePickerStyle&lt;S>(S) -> some View

Sets the style for date pickers within this view.

