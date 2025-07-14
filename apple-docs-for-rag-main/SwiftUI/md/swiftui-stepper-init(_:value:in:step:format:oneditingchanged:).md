

- SwiftUI
- Stepper
-  init(\_:value:in:step:format:onEditingChanged:) 

Initializer

# init(\_:value:in:step:format:onEditingChanged:)

Creates a stepper instance that increments and decrements a binding to a value, by a step size and within a closed range that you provide, displaying its value with an applied format style.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    value: Binding,
    in bounds: ClosedRange,
    step: F.FormatInput.Stride = 1,
    format: F,
    onEditingChanged: @escaping (Bool) -> Void = { _ in }
) where F : ParseableFormatStyle, F.FormatInput : BinaryFloatingPoint, F.FormatOutput == String
```

Available when `Label` is `Text`.

Show all declarations

## Parameters 

`titleKey`  

The key for the stepper’s localized title describing the purpose of the stepper.

`value`  

A Binding to a value that your provide.

`bounds`  

A closed range that describes the upper and lower bounds permitted by the stepper.

`step`  

The amount to increment or decrement `value` each time the user clicks or taps the stepper’s increment or decrement button, respectively. Defaults to `1`.

`format`  

A format style of type `F` to use when converting between the string the user edits and the underlying value of type `F.FormatInput`. If `format` can’t perform the conversion, the stepper leaves `value` unchanged. If the user stops editing the text in an invalid state, the stepper updates the text to the last known valid value.

`onEditingChanged`  

A closure that’s called when editing begins and ends. For example, on iOS, the user may touch and hold the increment or decrement buttons on a `Stepper` which causes the execution of the `onEditingChanged` closure at the start and end of the gesture.

## Discussion

Use `Stepper(_:value:in:step:format:onEditingChanged:)` to create a stepper that increments or decrements a value within a specific range of values by a specific step size, while displaying the current value. In the example below, a stepper increments or decrements a binding to value over a range of `1...50` by `5` each time the user clicks or taps the stepper’s increment or decrement buttons:

```
struct StepperView: View {
    @State private var value = 0

    var body: some View {
        Stepper("Stepping by \(step) in \(range.description)",
            value: $value,
            in: 1...50,
            step: 5,
            format: .number
        )
        .padding()
    }
}
```

## See Also

### Creating a stepper over a range

init&lt;V>(value: Binding&lt;V>, in: ClosedRange&lt;V>, step: V.Stride, label: () -> Label, onEditingChanged: (Bool) -> Void)

Creates a stepper configured to increment or decrement a binding to a value using a step value and within a range of values you provide.

init&lt;F>(value: Binding&lt;F.FormatInput>, in: ClosedRange&lt;F.FormatInput>, step: F.FormatInput.Stride, format: F, label: () -> Label, onEditingChanged: (Bool) -> Void)

Creates a stepper configured to increment or decrement a binding to a value using a step value and within a range of values you provide, displaying its value with an applied format style.

init(_:value:in:step:onEditingChanged:)

Creates a stepper instance that increments and decrements a binding to a value, by a step size and within a closed range that you provide.

