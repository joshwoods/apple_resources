

- SwiftUI
- Stepper
-  init(\_:value:step:format:onEditingChanged:) 

Initializer

# init(\_:value:step:format:onEditingChanged:)

Creates a stepper with a title key and configured to increment and decrement a binding to a value and step amount you provide, displaying its value with an applied format style.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    value: Binding,
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

A Binding to a value that you provide.

`step`  

The amount to increment or decrement `value` each time the user clicks or taps the stepper’s plus or minus button, respectively. Defaults to `1`.

`format`  

A format style of type `F` to use when converting between the string the user edits and the underlying value of type `F.FormatInput`. If `format` can’t perform the conversion, the stepper leaves `value` unchanged. If the user stops editing the text in an invalid state, the stepper updates the text to the last known valid value.

`onEditingChanged`  

A closure that’s called when editing begins and ends. For example, on iOS, the user may touch and hold the increment or decrement buttons on a `Stepper` which causes the execution of the `onEditingChanged` closure at the start and end of the gesture.

## Discussion

Use `Stepper(_:value:step:onEditingChanged:)` to create a stepper with a custom title that increments or decrements a binding to value by the step size you specify, while displaying the current value.

In the example below, the stepper increments or decrements the binding value by `5` each time the user clicks or taps on the control’s increment or decrement buttons, respectively:

```
struct StepperView: View {
    @State private var value = 1

    var body: some View {
        Stepper("Stepping by \(step)",
            value: $value,
            step: 5,
            format: .number
        )
        .padding(10)
    }
}
```

## See Also

### Creating a stepper

init&lt;V>(value: Binding&lt;V>, step: V.Stride, label: () -> Label, onEditingChanged: (Bool) -> Void)

Creates a stepper configured to increment or decrement a binding to a value using a step value you provide.

init&lt;F>(value: Binding&lt;F.FormatInput>, step: F.FormatInput.Stride, format: F, label: () -> Label, onEditingChanged: (Bool) -> Void)

Creates a stepper configured to increment or decrement a binding to a value using a step value you provide, displaying its value with an applied format style.

init(_:value:step:onEditingChanged:)

Creates a stepper with a title and configured to increment and decrement a binding to a value and step amount you provide.

