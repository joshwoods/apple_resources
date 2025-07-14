

- SwiftUI
- Stepper
-  init(\_:value:step:onEditingChanged:) 

Initializer

# init(\_:value:step:onEditingChanged:)

Creates a stepper with a title and configured to increment and decrement a binding to a value and step amount you provide.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    _ title: S,
    value: Binding,
    step: V.Stride = 1,
    onEditingChanged: @escaping (Bool) -> Void = { _ in }
) where S : StringProtocol, V : Strideable
```

Available when `Label` is `Text`.

Show all declarations

## Parameters 

`title`  

A string describing the purpose of the stepper.

`value`  

The Binding to a value that you provide.

`step`  

The amount to increment or decrement `value` each time the user clicks or taps the stepper’s increment or decrement button, respectively. Defaults to `1`.

`onEditingChanged`  

A closure that’s called when editing begins and ends. For example, on iOS, the user may touch and hold the increment or decrement buttons on a `Stepper` which causes the execution of the `onEditingChanged` closure at the start and end of the gesture.

## Discussion

Use `Stepper(_:value:step:onEditingChanged:)` to create a stepper with a custom title that increments or decrements a binding to value by the step size you specify.

In the example below, the stepper increments or decrements the binding value by `5` each time one of the user clicks or taps the control’s increment or decrement buttons:

```
struct StepperView: View {
    @State private var value = 1
    let step = 5
    let title: String

    var body: some View {
        Stepper(title, value: $value, step: step)
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

init(_:value:step:format:onEditingChanged:)

Creates a stepper with a title key and configured to increment and decrement a binding to a value and step amount you provide, displaying its value with an applied format style.

